# Third-Party Rerun Protocol

1. Clone the repository.
2. Run `bash repro/run_repro.sh`.
3. Confirm that `repro/certificate_runtime.json` reports `MSV_G1` through `MSV_G6` and `MSV_GM` as `PASS`.
4. Confirm that `scripts/release_gate.py --mode fully_extracted` returns `ok = true`.
5. Confirm that all tracked hashes in `repro/repro_manifest.json` match.
