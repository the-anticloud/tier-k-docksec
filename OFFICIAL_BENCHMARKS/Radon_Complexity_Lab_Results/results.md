# Radon_Complexity_Lab_Results
**Project:** `K_DOCKSEC` | **Status:** `PASS` | **Run:** `2026-09-30T17:14:20.030944+00:00`

**Framework:** [Radon — Cyclomatic Complexity & Maintainability Index](https://radon.readthedocs.io/)

## Key Metrics

- **files_analyzed:** `5`
- **average_complexity:** `{'grade': 'A', 'score': 3.268041237113402}`
- **complexity_grade:** `A`
- **complexity_score:** `3.268041237113402`
- **mi_output:** `E:\fenta\Downloads\The Anticloud\TIER_6_SECURITY_EVAL\K_DOCKSEC\UPSTREAM\_anticloud_egress.py - A (79.55)
E:\fenta\Downl`

## Raw Output (first 50 lines)
```
E:\fenta\Downloads\The Anticloud\TIER_6_SECURITY_EVAL\K_DOCKSEC\UPSTREAM\_anticloud_egress.py
    F 38:0 _is_frontier - A (4)
    F 43:0 guarded_connect - A (4)
    F 61:0 install - A (3)
    F 33:0 is_offline - A (1)
    C 29:0 EgressDenied - A (1)
E:\fenta\Downloads\The Anticloud\TIER_6_SECURITY_EVAL\K_DOCKSEC\UPSTREAM\pkg\fanal\analyzer\language\c\conan\testdata\cacheDir\.conan\data\openssl\3.0.5\_\_\export\conanfile.py
    M 342:4 OpenSSLConan._configure_args - D (22)
    M 532:4 OpenSSLConan.package - C (15)
    M 417:4 OpenSSLConan._create_targets - B (10)
    M 622:4 OpenSSLConan.package_info - B (8)
    M 322:4 OpenSSLConan._ancestor_target - B (6)
    M 118:4 OpenSSLConan.build_requirements - A (5)
    M 129:4 OpenSSLConan.validate - A (5)
    M 481:4 OpenSSLConan._run_make - A (5)
    C 17:0 OpenSSLConan - A (4)
    M 189:4 OpenSSLConan._asm_target - A (4)
    M 218:4 OpenSSLConan._targets - A (4)
    M 497:4 OpenSSLConan._make - A (4)
    M 96:4 OpenSSLConan.config_options - A (3)
    M 157:4 OpenSSLConan._target - A (3)
    M 166:4 OpenSSLConan._perlasm_scheme - A (3)
    M 108:4 OpenSSLConan.configure - A (2)
    M 114:4 OpenSSLConan.requirements - A (2)
    M 141:4 OpenSSLConan._is_clangcl - A (2)
    M 145:4 OpenSSLConan._is_mingw - A (2)
    M 149:4 OpenSSLConan._use_nmake - A (2)
    M 336:4 OpenSSLConan._get_default_openssl_dir - A (2)
    M 405:4 OpenSSLConan.generate - A (2)
    M 492:4 OpenSSLConan._perl - A (2)
    M 523:4 OpenSSLConan._make_program - A 
```

---
_Anticloud Independent Benchmark — 2026-09-30T17:14:20.030944+00:00_