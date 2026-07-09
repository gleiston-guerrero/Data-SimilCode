# Changelog

All notable changes to this dataset will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

- Zenodo DOI to be substituted in `README.md` and `CITATION.cff` once the
  v1.0.0 release is archived and its DOI is minted.
- Cross-repository *Related Identifiers* links to `BackEnd-SimilCode`
  (10.5281/zenodo.21265178), `FrontEnd-SimilCode` (10.5281/zenodo.21265977),
  and `SimilCode-Benchmark` (DOI pending) to be configured on the Zenodo record
  after minting (not embedded in `CITATION.cff` due to a known Zenodo
  InvenioRDM parser incompatibility with the `references:` block).

## [1.0.0] - 2026-07-09

Initial public release. Companion validation dataset for the manuscript
submitted to the *International Journal for Educational Integrity*
(Springer Nature).

### Added

- `README.md` — Dataset overview, repository structure, ethics statement,
  citation guidelines, and full author roster with verified ORCIDs.
- `LICENSE` — Creative Commons Attribution 4.0 International (CC BY 4.0),
  with SPDX identifier `CC-BY-4.0`.
- `CITATION.cff` — Machine-readable citation metadata in Citation File
  Format v1.2.0; five authors with confirmed ORCIDs; `type: dataset`.
- `instrument/` — Blank data-collection instruments used in the study,
  bilingual (Spanish original and English translation):
  - Informed-consent forms for the 2025 exploratory interview phase.
  - Informed-consent forms for the 2026 SimilCode validation phase.
  - 18-item structured questionnaire on a 5-point Likert scale, organised
    in three sections: practical usefulness (Q01–Q07), accuracy of results
    (Q08–Q13), and comprehensibility of justifications (Q14–Q18).
  - Four-dimension rubric (correctness, specificity, completeness, clarity)
    for the assessment of justification quality.
- `responses/` — Anonymised responses of the five-expert panel (P01–P05)
  from the Faculty of Computer Sciences at Universidad Técnica Estatal de
  Quevedo (UTEQ), Ecuador:
  - `responses_anonymised_wide.csv` — one row per participant, 18 Likert
    items plus non-identifying demographic covariates.
  - `responses_anonymised_long.csv` — tidy long format, 90 rows
    (5 participants × 18 items).
  - `codebook.csv` — variable dictionary.

### Ethics and privacy

- All raw response documents were anonymised prior to inclusion in this
  repository: names, national ID numbers (cédula), email addresses, phone
  numbers, handwritten signatures, exact participation dates, and any
  free-text identifiers were removed; participants are represented only
  by the codes P01–P05.
- The five participants provided written informed consent in accordance
  with the institutional ethical research guidelines of Universidad
  Técnica Estatal de Quevedo (UTEQ).
- No student-submitted code was used in the validation exercise; the code
  pairs shown to experts were drawn from the SimilCode benchmark corpus
  (see companion repository `SimilCode-Benchmark`).

[Unreleased]: https://github.com/gleiston-guerrero/SimilCode-Validation/compare/v1.0.0...HEAD
[1.0.0]: https://github.com/gleiston-guerrero/SimilCode-Validation/releases/tag/v1.0.0