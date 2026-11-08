# L5 Narrow / L2 General Classification — K_DOCKSEC
**Platform:** Anticloud | **Tier:** TIER_6_SECURITY_EVAL | **PAX:** 27B
**IP:** USPTO pending 2026, Anticloud FZ LLE, 0-1.gg | **License:** Apache-2.0

## L5 Narrow
K_DOCKSEC evaluates Docker container security for Anticloud deployments: image vulnerability scanning, container configuration hardening, runtime security policy enforcement. Narrow scope: Anticloud container security only.

## L2 General
L2 General: K_DOCKSEC secures all containerized Anticloud deployments (TIER_3 docker-compose, TIER_3 kubernetes-manifests). Same container security evaluation for hospital and defense deployments.

## PAX 27B Integration
PAX 27B analyzes Trivy scan results and generates prioritized remediation plans: given a list of CVEs, PAX ranks them by exploitability in the Anticloud context and suggests fixes.

## AIOSS Audit Chain
Every container security scan (image hash + CVE findings hash + CIS benchmark score + remediation plan hash) is chained: H_n = SHA3-256(H_{n-1} || entry_hash_n || timestamp_n).
Offline-verifiable, tamper-evident, zero cloud dependency.

## Regulatory / Compliance
CIS Docker Benchmark, NIST SP 800-190 (container security), CVE.
