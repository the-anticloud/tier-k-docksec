# Deploy Guide — K_DOCKSEC
**Tier:** TIER_6_SECURITY_EVAL | **Stack:** Python 3.11, docker SDK, trivy (container scanner), PAX 27B, AIOSS_FORMAT
**Air-gap capable after initial setup.**

## Prerequisites
Python 3.11+, docker SDK 7.0+, trivy 0.50+ (binary), PAX 27B.

## Environment
Docker daemon running. Trivy binary installed. GPU for PAX remediation analysis.

## AIOSS Integration
```bash
aioss init --module K_DOCKSEC --output ./k_docksec.aioss
aioss append --chain ./k_docksec.aioss --payload ./output.bin --module K_DOCKSEC
aioss verify --chain ./k_docksec.aioss
```

## Air-Gap Setup
```bash
pip download -r requirements.txt -d ./wheels/
pip install --no-index --find-links ./wheels/ -r requirements.txt
```

## PAX 27B Harness Wiring
```python
from anticloud_pax import PAXHarness
harness = PAXHarness(
    model_path="./pax-27b-q4.gguf",
    module="K_DOCKSEC",
    aioss_chain="./K_DOCKSEC.aioss",
    classification="L5_NARROW_L2_GENERAL"
)
result = harness.process(input_data)
```

## Verification
```bash
aioss verify --chain ./K_DOCKSEC.aioss --verbose
python -m K_DOCKSEC.tests.smoke
```
