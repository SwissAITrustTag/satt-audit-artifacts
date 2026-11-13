# Swiss AI Trust Tag (SATT) — Public Audit Artifacts & Cryptographic Manifests

**Official Cryptographic Verification Repository for SATT Deterministic Evaluations**  
📍 Zurich, Switzerland | 🌐 [swissaitrusttag.ch](https://swissaitrusttag.ch)

---

## Purpose of This Repository

This repository hosts versioned cryptographic manifests (`SHA-256` digests, Merkle roots, deterministic seeds, and statistical adjudication summaries) for published **Swiss AI Trust Tag (SATT)** foundation model audits.

Every benchmark published on [swissaitrusttag.ch](https://swissaitrusttag.ch) is executed and sealed locally under strict Zero-Trust isolation. Researchers, enterprise compliance teams, and model vendors can verify the integrity of evaluation artifacts against the cryptographic digests recorded in this repository.

---

## Audit Registry

| Audit ID | Target Benchmark | Models Evaluated | Evaluation Regime | Status | Directory |
| :--- | :--- | :--- | :--- | :---: | :--- |
| **`SATT-T-2026-001`** | MMLU-Pro (1,684 Stratified Items) | `google/gemini-4-carbon`<br>`google/gemini-4-argon` | Paired Item-Level Deterministic Evaluation | `SEALED & PUBLISHED` | [`/audits/SATT-T-2026-001`](./audits/SATT-T-2026-001) |
| **`SATT-T-2026-002`** | CWE-bench (Public Dataset) | `google/gemini-4-carbon`<br>`google/gemini-4-argon`<br>`google/gemini-4-hydrogen` | Multi-Turn Agentic Docker Remediation | `ACTIVE CALIBRATION` | [`/audits/SATT-T-2026-002`](./audits/SATT-T-2026-002) |

---

## Core Verification Standards

- **Statistical Adjudication:** Paired item-level testing using exact McNemar p-values, 95% Wilson confidence intervals, and predefined Region of Practical Equivalence (ROPE) bounds.
- **Cryptographic Sealing:** Raw model rollouts, container verifier logs, and dataset snapshots are hashed with `SHA-256` and bound into a verifiable Merkle root.
- **Neutral Governance:** SATT operates as a neutral, empirical verification authority based in Zurich, Switzerland.
