# SATT Cryptographic & Statistical Verification Protocol

## 1. Local Artifact Integrity (`SHA-256` and Merkle Root)

Every SATT audit produces a canonical JSON manifest containing:

1. **Dataset Snapshot Digest:** The `SHA-256` hash of the exact input evaluation items (`items.jsonl`) and deterministic sampling seed.
2. **Rollout and Verifier Digests:** `SHA-256` hashes of raw model responses and isolated container execution logs.
3. **Merkle Root:** A binary Merkle tree root computed over all sorted artifact digests in the audit bundle.

To verify a published SATT artifact locally:

```bash
sha256sum <artifact_filename>
```

Compare the resulting 64-character hexadecimal digest with the manifest published in the corresponding `/audits/SATT-T-2026-XXX/` directory and on [swissaitrusttag.ch](https://swissaitrusttag.ch).

## 2. Paired Statistical Adjudication

SATT uses paired item-level evaluation instead of aggregate leaderboard comparisons:

- **95% Wilson Score Interval:** Used for binomial accuracy bounds on finite samples.
- **Exact McNemar Test:** Evaluates discordant pairs (Model A pass / Model B fail versus Model A fail / Model B pass) to determine statistical significance.
- **ROPE (Region of Practical Equivalence):** Uses a predefined equivalence margin (for example, ±1.0 percentage point) to distinguish practically equivalent outcomes from operationally meaningful differences.
