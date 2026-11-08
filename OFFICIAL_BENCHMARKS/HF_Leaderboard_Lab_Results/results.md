# HF_Leaderboard_Lab_Results

**Project:** `K_DOCKSEC`  
**Tier:** `TIER_6_SECURITY_EVAL`  
**Slug:** `aquasecurity/trivy`  
**Commit:** `3a1b311e63a1`  
**Run:** `2026-09-30T15:07:07.146295+00:00`  

## Isolation Environment

| Field | Value |
| ----- | ----- |
| Platform | `win32` |
| Python | `3.12.10` |
| HF model | `distilbert-base-uncased` |
| HF load time | `4.42s` |
| Inference device | `cpu` |

## Results

**Framework:** [HuggingFace Open LLM Leaderboard (proxy via distilbert-base-uncased)](https://huggingface.co/docs/leaderboards/en/open_llm_leaderboard/archive)

**Model used:** `distilbert-base-uncased`

### Inference Latency (Classification)

| Metric | Value |
| ------ | ----- |
| Avg latency | **47.68 ms** |
| Min latency | 45.0 ms |
| Max latency | 52.41 ms |
| Samples | 5 |

### Real Tokenization Results

| Field | Value |
| ----- | ----- |
| Token count | **40** |
| Tokenization latency | 0.0 ms |
| Classification label | `LABEL_0` |
| Classification score | 0.5842 |
| Classification latency | 83.95 ms |
| Status | **PASS** |

**Input text tokenized:**
```
K_DOCKSEC (aquasecurity/trivy) — 3400 files, 283269 source lines, licence Apache-2.0, primary language ['Go']
```

**First 20 tokens:**
```
['[CLS]', 'k', '_', 'docks', '##ec', '(', 'aqua', '##se', '##cu', '##rity', '/', 'tri', '##vy', ')', '—', '340', '##0', 'files', ',', '283']
```

> Full MMLU/HellaSwag/TruthfulQA/ARC/Winogrande/GSM8K require dedicated GPU.
> These results are CPU inference proxy metrics using distilbert-base-uncased.

---
_Anticloud Benchmark Suite — isolation log — 2026-09-30T15:07:07.146295+00:00_