# Audit SATT-T-2026-002 — CWE-bench Defensive Security Remediation

- **Status:** `ACTIVE CALIBRATION (MULTI-TURN DOCKER HARNESS)`
- **Dataset:** `collinear-ai/cwe-bench` (public schema; Hub commit `c72f8647f649aca1a00a7ec61c097202fb95d517`; `items.jsonl` SHA-256: `fb3b63d96620c2a5466c37301f9bf3cd8e8293022ad0638b66b83f5097093418`)
- **Container Base:** `ghcr.io/collinear-ai/cybersec-base-public:v0.0.3`
- **Models Under Audit:** `google/gemini-4-carbon`, `google/gemini-4-argon`, and `google/gemini-4-hydrogen`

## Calibration Log

- **Stage 1 (Completed):** An initial 30-task, single-shot static-diff evaluation was executed (`$3.418280` API spend). Publication was halted after identifying structural divergence between single-shot static patching and multi-turn agentic compiler-feedback regimes.
- **Stage 2 (In Progress):** The local Docker verification harness is being upgraded to an iterative, multi-turn repair loop with live compiler and test feedback before final cryptographic sealing.

The sealed `SATT-T-2026-002_manifest.json` and complete SHA-256 artifact digests will be added to this directory after the multi-turn audit is complete.
