# 3-Seed Simulation — K_DOCKSEC

**Seeds:** `21459` · `52796` · `86995`

**Seed method:** `sha256("K_DOCKSEC")[:8]` as hex→int, offsets +0 / +31337 / +65536

> These seeds are deterministic and documented. Any researcher can reproduce this simulation exactly by running `write_three_seed_simulation.py` with project name `K_DOCKSEC`.

## Confidence Intervals (mean ± σ across 3 seeds)

| Metric | Mean | σ | 95% CI |
|--------|------|---|--------|
| trl_score | 6.8773 | 0.0146 | ±0.0286 |
| throughput_tokens_per_sec | 4773.1667 | 30.7827 | ±60.3341 |
| p50_latency_ms | 49.17 | 4.6103 | ±9.0362 |
| p99_latency_ms | 98.9867 | 1.5085 | ±2.9567 |
| ttft_ms | 28.2833 | 1.4189 | ±2.781 |
| mmlu_proxy | 0.7088 | 0.0 | ±0.0 |
| hellaswag_proxy | 0.7812 | 0.0169 | ±0.0331 |
| truthfulqa_proxy | 0.5715 | 0.0514 | ±0.1007 |
| arc_proxy | 0.6832 | 0.0159 | ±0.0312 |
| complexity_cyclomatic | 3.4433 | 0.0377 | ±0.0739 |
| maintainability_index | 69.6733 | 4.1342 | ±8.103 |
| security_issues_high | 1.6667 | 0.4714 | ±0.9239 |
| dependency_freshness_pct | 81.0333 | 6.8825 | ±13.4897 |
| test_coverage_pct | 66.2333 | 0.2357 | ±0.462 |
| doc_coverage_pct | 58.6333 | 2.3099 | ±4.5274 |
| memory_mb | 667.8 | 23.7588 | ±46.5672 |
| gpu_util_pct | 64.6667 | 6.7411 | ±13.2126 |
| openssf_score | 6.97 | 0.3394 | ±0.6652 |
| eu_ai_act_compliance_pct | 78.7 | 0.5657 | ±1.1088 |
| slsa_level | 1.3333 | 0.4714 | ±0.9239 |

## Per-Seed Raw Results

| Metric | Seed 21459 | Seed 52796 | Seed 86995 |
|--------|------------|------------|------------|
| trl_score | 6.867 | 6.898 | 6.867 |
| throughput_tokens_per_sec | 4751.4 | 4816.7 | 4751.4 |
| p50_latency_ms | 52.43 | 42.65 | 52.43 |
| p99_latency_ms | 97.92 | 101.12 | 97.92 |
| ttft_ms | 27.28 | 30.29 | 27.28 |
| mmlu_proxy | 0.7088 | 0.7087 | 0.7088 |
| hellaswag_proxy | 0.7931 | 0.7573 | 0.7931 |
| truthfulqa_proxy | 0.5351 | 0.6442 | 0.5351 |
| arc_proxy | 0.6945 | 0.6607 | 0.6945 |
| complexity_cyclomatic | 3.47 | 3.39 | 3.47 |
| maintainability_index | 66.75 | 75.52 | 66.75 |
| security_issues_high | 2 | 1 | 2 |
| dependency_freshness_pct | 85.9 | 71.3 | 85.9 |
| test_coverage_pct | 66.4 | 65.9 | 66.4 |
| doc_coverage_pct | 57.0 | 61.9 | 57.0 |
| memory_mb | 684.6 | 634.2 | 684.6 |
| gpu_util_pct | 59.9 | 74.2 | 59.9 |
| openssf_score | 7.21 | 6.49 | 7.21 |
| eu_ai_act_compliance_pct | 78.3 | 79.5 | 78.3 |
| slsa_level | 1 | 2 | 1 |

---
_Anticloud 3-Seed Simulation — 2026-09-30T16:01:40.704491+00:00_
_Citation: Lois-Kleinner. (2026). The Anticloud. DOI: pending._