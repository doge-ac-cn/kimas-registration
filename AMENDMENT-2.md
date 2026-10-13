# AMENDMENT-2 — Protocol-layer closure (2026-10-13)

Sponsored by the round-3 + verification audits (docs/audit_final_v2.md second round; kimas_双智能体审计综合.md §五). Four documentation-level items, executed in one pass:

1. **SEAL.md §1**: actual seal-opening date recorded as 2026-10-12 (Amendment-1 accelerated window; original 2027-01-04 struck through, both visible). §6 change log: opening entry added.
2. **commitments.txt policy redesign**: the commitment file anchors **documents only** — proof files (.ots) are version-controlled repository files whose content legitimately changes upon Bitcoin confirmation; anchoring their hashes made confirmation itself break the commitment. All .ots hash lines removed; the v1 stamp retained as an archive file (commitments_v1_20261011.ots).
3. **Patient-naming glossary** (two generations of filename convention, resolution pending author confirmation):
   - Gen-1 names: `pN_IMG_CROP` (e.g., p1_0299_6) — first segment = patient (pN)
   - Gen-2 names: `NUM_SLIDE_CROP` (e.g., 12655_0299_1) — first segment = slide/accession, second segment = patient/case
   - Counts observed: first-segment parse → 23 segments in test256 (46 across both splits); second-segment parse → 305 patient IDs in test256 (373 in train256, 286 shared). True patient count pending author confirmation (requested in the acknowledgment letter).
   - E3 patient-level statistics reported under the conservative first-segment clustering (23 clusters, widest CI).
4. **Stale-statement corrections**: 46→23 patient count in m1_verdict_final.md / monitor_log / adapt docs; E2 report MAE-reduction figure dual-caliber (−39% within-set / −46% vs val baseline).

All items hash-committed below and OpenTimestamps-anchored. With this amendment, protocol-layer fixes are CLOSED; remaining pre-submission work is manuscript writing.
