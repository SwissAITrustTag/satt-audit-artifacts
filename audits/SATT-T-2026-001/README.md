# Audit SATT-T-2026-001 — MMLU-Pro Deterministic Comparison

- **Status:** `SEALED & PUBLISHED`
- **Benchmark Dataset:** MMLU-Pro (`1,684` stratified evaluation items)
- **Models Evaluated:** `google/gemini-4-carbon` versus `google/gemini-4-argon`
- **Evaluation Regime:** Paired Item-Level Deterministic Evaluation
- **Full Sealed Report:** [swissaitrusttag.ch](https://swissaitrusttag.ch/benchmarks/SATT-T-2026-001-v1)

---

## Key Verified Summary

| Model Slug | Stratified Items | Accuracy (%) | Verified API Spend (USD) | SATT Adjudication Verdict |
| :--- | :---: | :---: | :---: | :--- |
| `google/gemini-4-carbon` | 1,684 | **91.1%** | $14.73 | Statistically Indistinguishable Tier |
| `google/gemini-4-argon` | 1,684 | **91.1%** | $6.87 | Optimal Cost-Efficiency Tier (~2.14× lower spend) |

---

## Verification Notes

This directory archives the public verification metadata for Audit **`SATT-T-2026-001`**. Full cryptographic digests (`SHA-256` and Merkle root), paired McNemar statistics, and item-level breakdowns are published and verifiable through the official SATT portal at [swissaitrusttag.ch](https://swissaitrusttag.ch/benchmarks/SATT-T-2026-001-v1).
