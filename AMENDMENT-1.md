# AMENDMENT 1 — Execution window accelerated (2026-10-12)

The development phase completed approximately two months ahead of the original schedule. As of 2026-10-12 the system is declared FINAL:

- Detector (A1): Faster R-CNN R50-FPN, checkpoint epoch040 (seed 42), SHA-256 25ac3dc1ef0de8a57163c88b6b89272d86201e88ad11d5a7f38495b02816162c
- Second reader (A3): Qwen3-VL-8B qLoRA adapter, checkpoint-300, SHA-256 8b58caf0b6a11afa7fac0f20451f1665b3c2e790f3d203a7053bee3910b7e871
- Selection stage (A2): rule-based champion arm (heatmap-threshold), per the registered four-arm comparison outcome (learnable variant reported transparently)
- Arbitration (A4): delta_low=15pp / delta_high=18pp (val-calibrated), conformal alpha=0.10 (val q=10.14pp, coverage 91.7%)

The confirmatory sealed run (BCData-402 + SHIDC V1.1 + comparison table) will execute as a single pre-specified run immediately following this amendment, upon investigator authorization. Outcomes stand regardless of result; no re-run, no tuning on sealed test sets.

All other terms of the registered plan remain in force. E12 seed-replication (seeds 42/43/44) completed: val mAP range 0.5pp, F1 range <=0.9pp, PI R^2 range 1.3pp (frozen seed-42 model used for the sealed run).

This amendment is hash-committed and OpenTimestamps-anchored like the original registration.
