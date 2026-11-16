# Lorenzo Vasile

Computer Science undergraduate at the University of Palermo (Class of 2028), currently spending the Fall 2026 semester at the University of Granada (ETSIIT) through Erasmus+.

I mostly work on **C/C++, Linux systems, ARM64 hardware, and cross-platform developer tooling**. I am currently looking for **Summer 2027** software and systems engineering internships in Europe (available July–October 2027, EU citizen).

## Selected work

- **[PradoOS (`prado-os`)](https://github.com/LorSt4r/prado-os)** · [PyPI](https://pypi.org/project/prado-os/) — Local-first synchronization engine and native Menu Bar / System Tray app for UGR's PRADO (Moodle) platform across macOS, Linux, and Windows (`AGPLv3`). Built to automate course material sync without ever overwriting local student edits (4-quadrant SHA-256 + SQLite conflict resolution). Includes a 3-tier headless SAML 2.0 + MFA login pipeline backed by native OS keyrings (`Keychain`, `Credential Manager`, `SecretService` + AES-256 fallback), an `IMAP4_SSL`/`SMTP_SSL` institutional mail client, zero-dependency Google Calendar v3 OAuth2 sync, background OS daemons (`launchd`, `systemd`, `schtasks`), and 764+ `pytest` unit, adversarial, and live E2E tests across a 3-OS GitHub Actions matrix. Currently under institutional evaluation with the University of Granada's Open Source Office (OSL) and CEPRUD.
- **[`ik_llama.cpp` (Open Source)](https://github.com/ikawrakow/ik_llama.cpp)** — Upstream contributions to the C/C++ LLM inference engine:
  - **[PR #2094 (Merged)](https://github.com/ikawrakow/ik_llama.cpp/pull/2094):** Fixed CMake build flag propagation to enable native ARM64 `+dotprod` SIMD kernels and resolved GCC 14 `<cstdint>` / macro issues on Neoverse cores.
  - **[PR #2410 (Merged)](https://github.com/ikawrakow/ik_llama.cpp/pull/2410):** Fixed a circular token-history buffer eviction bug in C++ that broke repetition penalties at capacity boundaries, adding a deterministic unit regression harness.
- **[ARM64 LLM Inference Lab](https://github.com/LorSt4r/arm64-llm-inference-lab)** — Reproducible benchmark setup and profiling notes for CPU-only quantized inference (`Qwen3.6-35B-A3B` via `ik_llama.cpp`) on a 4-OCPU, 24 GiB RAM Oracle Ampere A1 Linux instance. Tuned `mlock` and cache allocation to drop swap usage from 571 MiB to 0 MiB and increase sustained decoding throughput by 23% (7.27 vs 5.92 tokens/s).
- **[Sauta](https://github.com/LorSt4r/sauta-platform)** — Multi-tenant venue operations backend built with TypeScript, Fastify, PostgreSQL, Prisma, and Docker, implementing tenant boundary isolation, RBAC, idempotent webhook handling, and automated CI test pipelines.
- **[Chess to Lichess](https://github.com/LorSt4r/ChessToLichess)** — Manifest V3 Chrome extension ([Chrome Web Store](https://chromewebstore.google.com/detail/chess-to-lichess/bmjpmngmefogekoellogiaeldplnbcia)) that exports finished Chess.com games directly to Lichess engine analysis.

## Toolkit

- **Languages:** C, C++, Python, SQL (SQLite, PostgreSQL), Bash, PowerShell, TypeScript, JavaScript.
- **Systems & Infrastructure:** Linux (Debian/Ubuntu, ARM64), macOS, Windows, CMake, OS Daemons (`systemd`, `launchd`, `schtasks`), Docker, Git, GitHub Actions (multi-OS CI/CD), `llama.cpp` / GGUF.
- **Security, Protocols & Testing:** SAML 2.0 SSO & MFA, OAuth2, `IMAP4_SSL` / `SMTP_SSL`, OS Native Keyrings & AES-256/SHA-256, `pytest`, Vitest, Playwright.

## Contact

- **LinkedIn:** [linkedin.com/in/lorenzovasile07](https://www.linkedin.com/in/lorenzovasile07)
- **Email:** [lorenzovasile07@gmail.com](mailto:lorenzovasile07@gmail.com)
