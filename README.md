# KiMAS — Registered Confirmatory Analysis Plan (hash commitment)

**Domain**: computational pathology — automated Ki-67 proliferation index quantification in breast cancer IHC (breast cancer, immunohistochemistry, digital pathology, AI).

**What this repository is**: a public, timestamped commitment to the registration documents of a sealed confirmatory study. The full documents are held privately and will be published at preprint submission; anyone can then verify them against the SHA-256 commitments in `commitments.txt`.

**Study summary (deliberately mechanism-level-vague; details in the committed documents)**: a multi-stage automated system estimates the Ki-67 proliferation index from IHC whole-slide-derived imagery. The study follows a two-phase protocol: (1) a development phase on public training/validation splits, completed 2026-10; (2) a **sealed confirmatory phase** on held-out test sets whose archives were hashed and frozen before any access — to be opened and analyzed in a single pre-specified run in January 2027. Primary endpoints (detection metrics, index-agreement metrics vs. published anchors, evidence-recomputation audit rate, uncertainty-coverage targets) and all frozen hyperparameters are fixed in the committed registration documents.

**Datasets**: BCData (Huang et al., ECCV 2020) held-out test split; SHIDC-B-Ki-67 V1.1 (Negahbani et al., Sci Rep 2021) as external validation, obtained from the dataset authors under their terms of use; Patherea corrected evaluation protocol (Steperc et al.) adopted for detector comparison.

**Why hash-commitment instead of a full public preregistration**: the study's competitive window requires the mechanism details to remain non-public until the preprint; the commitment proves existence and immutability of the complete plan without disclosure.

**Verification**:
1. `sha256sum` each document after publication and compare with `commitments.txt`.
2. `commitments.txt` is anchored via OpenTimestamps (Bitcoin-anchored proof of existence time, independent of this hosting); verify with `ots verify`.

**Timeline**: registered 2026-10-12 (see `commitments.txt` generation time and OpenTimestamps proofs). Seal opening 2027-01-04. Preprint target 2027-02-15 to 2027-02-21, at which time the full registration documents are published here.

**License**: the commitment texts are CC0. (No code or data in this repository.)
