# Developer Cookbook — K_DOCKSEC
**Stack:** Python 3.11, docker SDK, trivy (container scanner), PAX 27B, AIOSS_FORMAT
**Domain:** Docker security evaluation for Anticloud containerized deployments

## Scan Anticloud containers
```python
from k_docksec import DockerSecurityEvaluator

evaluator = DockerSecurityEvaluator(
    pax_model="./pax-27b-q4.gguf",
    aioss_chain="./docksec.aioss"
)

result = evaluator.scan(image="anticloud/pax-inference:latest")
print(f"CRITICAL: {result.critical_cves}, HIGH: {result.high_cves}")

# PAX remediation plan
remediation = evaluator.pax_remediation_plan(result)
for item in remediation.actions:
    print(f"[{item.priority}] {item.action}")
    print(f"  Dockerfile fix: {item.dockerfile_change}")

# CIS benchmark score
cis_score = evaluator.cis_benchmark_score()
print(f"CIS score: {cis_score.passed}/{cis_score.total}")
```

## AIOSS Chain Append
```python
import hashlib, time

def aioss_append(chain_path, payload: bytes, module_id: str):
    entry_hash = hashlib.sha3_256(payload).digest()
    ts = int(time.time_ns()).to_bytes(8, 'big')
    with open(chain_path, 'rb') as f:
        f.seek(-32, 2); prev_hash = f.read(32)
    new_hash = hashlib.sha3_256(prev_hash + entry_hash + ts).digest()
    with open(chain_path, 'ab') as f:
        f.write(ts + entry_hash + new_hash)
    return new_hash.hex()
```
