# Changelog

## 1.0.5 — 2026-08-27

### DOI / citation / bibliographic metadata patch

- records the Distribution `1.0.5` Zenodo version DOI `10.5281/zenodo.22129037`;
- preserves all-versions / concept DOI `10.5281/zenodo.22127380` for the existing Zenodo version chain;
- updates Japanese and English README DOI / Distribution metadata;
- updates `CITATION.md`, `CITATION.cff`, and `VERSION.md` for Distribution `1.0.5`;
- preserves the published `v1.0.4` GitHub tag, Release, archive, and Zenodo version record unchanged;
- keeps creator/licensor identity `639228` and license `CC BY 4.0` / `CC-BY-4.0` unchanged.

### Behavioral / semantic boundary

- Protocol `v8.3.18` unchanged;
- Trigger Index `v0.1` unchanged;
- Coverage / Manifest / Retrieval / Regression / Cross / Integration semantic/support identities unchanged;
- fresh behavioral rerun: `NO START`;
- no runtime loading, bootstrap, source-selection, dispatch, semantic-owner, minimum-runtime, or installation change;
- no semantic repair, new runtime operation, Trigger row, field 4/6 semantic change, Regression expectation change, or Reference Gate change.

## 1.0.4 — 2026-08-27

### License detection / metadata packaging patch

- replaced the mixed explanatory `LICENSE.md` with the standard Creative Commons Attribution 4.0 International license text;
- moved distribution-specific copyright, license-application scope, third-party-material boundary, attribution guidance, and no-endorsement guidance to new `NOTICE.md`;
- updated the Japanese README license/citation navigation to distinguish `LICENSE.md`, `NOTICE.md`, and `CITATION.md`;
- aligned Distribution metadata to `1.0.4`;
- preserved Creator / Licensor identity `639228` and license decision `CC BY 4.0` / `CC-BY-4.0`;
- intended GitHub metadata verification: repository license should resolve from `Other / NOASSERTION` to `Creative Commons Attribution 4.0 International / CC-BY-4.0` after publication and GitHub reindexing.

### Behavioral / semantic boundary

- Protocol `v8.3.18` unchanged;
- Trigger Index `v0.1` unchanged;
- Coverage / Manifest / Retrieval / Regression / Cross / Integration semantic/support identities unchanged;
- fresh behavioral rerun: `NO START`;
- no semantic repair, new runtime operation, Trigger row, field 4/6 semantic change, Regression expectation change, or Reference Gate change.



## 1.0.3 — 2026-08-27

### README quick-access / navigation patch

- added `Installation` and `Latest Release` links beside the existing `English` link at the top of the Japanese primary README;
- added a compact `最短で試す` section immediately after the opening problem statement and before `これは何か`;
- reused the established first-time four-file ChatGPT setup: `README.md`, `INSTALLATION.md`, Protocol, and Trigger Index;
- preserved Protocol + Trigger Index as the two-file minimum canonical runtime pair;
- linked the detailed guide with repository-relative `[INSTALLATION.md](INSTALLATION.md)` rather than a ChatGPT-internal Project/conversation URL;
- left the explanatory body otherwise unchanged.

### Behavioral / semantic boundary

- Protocol `v8.3.18` unchanged;
- Trigger Index `v0.1` unchanged;
- no new runtime operation, Trigger row, field 4/6 rule, Regression expectation, bootstrap semantic rule, or translated canonical runtime;
- new fresh behavioral run: `NO START`; this patch only creates a shorter navigation path to already documented loading instructions.

### Release state

- Distribution `1.0.3` is the published stable README quick-access/navigation documentation patch over `1.0.2`;
- GitHub tag/release `v1.0.3` is published and verified;
- `v1.0.3` is the current Latest Release;
- `v1.0.3` tag points to commit `2f86de4b966e7ee0d895e429db84bfc092cc5cfa`;
- published archive SHA-256 is `7a097b568b79a2df9b922223a40bff0028f44076afcfd6414ecd0fe083d0fc31`;
- Protocol remains `v8.3.18`; Trigger Index remains `v0.1`.

## 1.0.2 — 2026-08-27

### Public entrypoint / ChatGPT setup / repository metadata patch

- adopted the public-facing Japanese README prepared from the canonical Protocol's execution-control framing;
- moved the public entrypoint from package-description-first to problem → purpose → capability → use → installation;
- documented the distinction between ordinary capability prompts and runtime execution conditions;
- documented necessary-and-sufficient analysis rather than maximum analysis;
- added concrete use cases and a detailed ChatGPT Project setup path;
- standardized Japanese ChatGPT UI wording on `情報源`;
- made the first-time recommended ChatGPT setup four files: `README.md`, `INSTALLATION.md`, Protocol, and Trigger Index;
- preserved Protocol + Trigger Index as the two-file minimum canonical runtime pair;
- added `README.en.md` and `INSTALLATION.en.md` to the distribution package as English navigation/loading documents, not translated canonical runtime artifacts;
- recorded the assigned public repository URL: `https://github.com/639228/structural-reading-protocol`.

### Behavioral / semantic boundary

- Protocol `v8.3.18` unchanged;
- Trigger Index `v0.1` unchanged;
- Coverage / Manifest / Retrieval / Regression / Cross / Integration payloads unchanged;
- LICENSE, metadata authority, canonical handoff, SOURCE checksum inventory, and saved fresh execution evidence unchanged;
- README/INSTALLATION changes are downstream explanation/loading guidance and do not create a new runtime operation, Trigger row, field 4/6 rule, semantic owner, or translated canonical runtime;
- new fresh behavioral run: `NO START`; the recommended four-file first-time setup matches the already saved fresh-environment test input structure, while the runtime semantic pair remains unchanged.

### Release state

- Distribution `1.0.2` is the current stable documentation patch over `1.0.1`;
- GitHub publication of tag/release `v1.0.2` remains the next hosting step;
- Protocol remains `v8.3.18`; Trigger Index remains `v0.1`.

## 1.0.1 — 2026-08-26

### Documentation-only acknowledgement patch

- added a `謝辞` section to `README.md` recording author-supplied educational/intellectual provenance and gratitude concerning two already named direct transmission sources in the canonical Protocol: 佐々木寛 and 篠原成彦
- preserved the acknowledgement as non-normative downstream documentation; it does not assign authorship of the Protocol or later operational development to either person
- recorded `信州大学で学んでいた際に` as author-supplied contextual provenance in the README acknowledgement; this contextual statement is not treated as a new canonical Protocol claim
- updated Distribution identity from `1.0.0` to `1.0.1` and refreshed downstream current-state / capacity metadata
- added `release_control/WORK_UNIT_07_README_ACKNOWLEDGEMENT_PATCH.md`

### Verified preservation

- Protocol `v8.3.18` unchanged
- Trigger Index `v0.1` unchanged
- Coverage / Manifest / Retrieval / Regression / Cross / Integration payloads unchanged
- `INSTALLATION.md`, `LICENSE.md`, `CITATION.md`, metadata authority, and saved fresh execution evidence unchanged
- no runtime/bootstrap semantic rule added, removed, strengthened, or weakened
- no new Trigger row, runtime operation, field 4/6 semantic change, Regression expectation change, or semantic repair

### Fresh-deployment judgment

- new behavioral run: `NO START`
- reason: the only executable-facing substantive addition is a non-normative README acknowledgement; runtime files, installation path, bootstrap semantics, runtime-role guidance, necessity gating, and stop semantics are unchanged
- prior bounded fresh result remains `8 / 8 PREPARED FD CASES PASS` at its saved evidence strength

### Release state

- Distribution `1.0.1` is the current stable documentation patch over `1.0.0`
- Protocol remains `v8.3.18`; Trigger Index remains `v0.1`

## 1.0.0 — 2026-08-26

### Stable public-release promotion

- promoted verified Distribution `1.0.0-rc.1` to stable public Distribution `1.0.0`
- changed only downstream release/version/current-state documentation plus package checksum regeneration
- added `release_control/WORK_UNIT_06_STABLE_PUBLIC_RELEASE_PROMOTION.md`

### Verified preservation

- Protocol `v8.3.18` byte-identical to `1.0.0-rc.1`
- Trigger Index `v0.1` byte-identical to `1.0.0-rc.1`
- Coverage / Manifest / Retrieval / Regression / Cross / Integration payloads byte-identical to `1.0.0-rc.1`
- `INSTALLATION.md`, `LICENSE.md`, `CITATION.md`, metadata authority, and saved fresh execution evidence byte-identical to `1.0.0-rc.1`
- runtime ownership / non-checklist / evidence-boundary guidance preserved
- no semantic repair, new runtime operation, Trigger row, field 4/6 semantic change, or Regression expectation change

### Evidence boundary

- prior bounded fresh result remains `8 / 8 PREPARED FD CASES PASS` at its saved operator-transferred execution strength
- no additional fresh behavioral run was started for stable promotion because runtime/bootstrap behavior did not change
- this stable release does not establish protocol-wide adequacy, natural whole-protocol execution, cross-model/cross-environment reproducibility, absence of systematic weakness, historical firstness, or universal performance improvement

### Release state

- Distribution `1.0.0` is the stable public release for the current downstream canonical snapshot
- repository and DOI remain unassigned and are not blockers at current inputs
- Protocol remains `v8.3.18`; Trigger Index remains `v0.1`

## 1.0.0-rc.1 — 2026-08-26

### Release-candidate promotion

- promoted verified development package `0.1.0-dev.5` to explicit Distribution release candidate `1.0.0-rc.1`
- established intended stable successor `1.0.0`
- updated public/readiness/version metadata for release-candidate identity
- added `release_control/WORK_UNIT_05_RELEASE_CANDIDATE_PROMOTION.md`

### Verified preservation

- Protocol `v8.3.18` byte-identical to dev.5
- Trigger Index `v0.1` byte-identical to dev.5
- Coverage / Manifest / Retrieval / Regression / Cross / Integration payloads byte-identical to dev.5
- `INSTALLATION.md`, `LICENSE.md`, `CITATION.md`, metadata authority, and saved fresh execution evidence byte-identical to dev.5
- no runtime/bootstrap semantic rule added, removed, strengthened, or weakened
- no new Trigger row, runtime operation, field 4/6 semantic change, Regression expectation change, or semantic repair

### Evidence boundary

- prior bounded fresh result remains `8 / 8 PREPARED FD CASES PASS` at its saved operator-transferred execution strength
- no additional fresh behavioral run was started for this version-only/current-state documentation promotion
- protocol-wide adequacy, natural whole-protocol execution, cross-model/cross-environment reproducibility, and absence of systematic weakness remain unestablished

### Release state

- `1.0.0-rc.1` is a release candidate, not the final `1.0.0` public release
- no identified current blocker remains for an explicit stable `1.0.0` promotion decision, subject to final RC package verification and no new contrary input

## 0.1.0-dev.5 — 2026-08-26

### Added / integrated

- authoritative public Creator / Licensor identity: `639228`
- `LICENSE.md` using Creative Commons Attribution 4.0 International (`CC BY 4.0`)
- `CITATION.md` with preferred creator name and Protocol citation format
- `release_control/PUBLIC_LICENSE_AND_CITATION_AUTHORITY_v1.0.md` as downstream metadata authority
- current fresh-environment execution record: FD-01..FD-08 `8 / 8 PASS` at bounded operator-transferred execution strength

### Release-state delta

- prior fresh behavioral blocker remains closed at its saved bounded strength
- prior LICENSE blocker closed after authoritative metadata integration and package verification
- prior CITATION blocker closed after authoritative metadata integration and package verification
- package is ready for release-candidate promotion; `0.1.0-dev.5` itself remains development-versioned

### Preserved

- Protocol `v8.3.18` unchanged
- Trigger Index `v0.1` unchanged
- Coverage / Manifest / Retrieval / Regression / Cross / Integration canonical/support bytes unchanged
- `INSTALLATION.md` unchanged
- no new runtime operation, Trigger row, field 4/6 semantic change, Regression expectation change, or semantic repair
- bounded fresh success is not generalized to protocol-wide adequacy, natural whole-protocol execution, systematic-weakness absence, or cross-model/cross-environment reproducibility

## 0.1.0-dev.4 — 2026-08-26

### Confirmed

- active Project-source count is now 14 / 25 after the previously planned retirement cycle
- six predecessor distribution/release Project-source copies were retired while package/repository history remained preserved
- `CURRENT_RELEASE_READINESS_STATE` revision 1.1 is prepared as a one-for-one successor current-state owner

### Packaging/materialization repair

- detected a post-archive working-directory materialization drift in the dev.3 mutable directory view
- independently extracted and verified the dev.3 tar archive: 25 files present; all source and package checksum entries PASS
- rebuilt dev.4 from the verified archive extraction rather than from the drifted mutable working directory

### Preserved

- all ten foundational/current canonical/support/control owners unchanged
- Protocol `v8.3.18`, Trigger `v0.1`, and Regression semantic expectations unchanged
- fresh behavioral execution remains unperformed
- LICENSE and CITATION remain unresolved without authoritative owner input
- no canonical semantic repair authorized

## 0.1.0-dev.3 — 2026-08-25

### Added

- consolidated `release_control/CURRENT_RELEASE_READINESS_STATE.md` current-state owner candidate
- confirmed Project-source capacity state after retirement of initial-tree and intake-verification active copies
- explicit successor-retirement path for Work Unit 02 / Work Unit 03 after successor Project-source admission

### Preserved

- all ten foundational/current canonical/support/control owners unchanged
- fresh behavioral execution remains unperformed
- LICENSE and CITATION remain unresolved without authoritative owner input
- no canonical semantic repair authorized



This changelog tracks downstream distribution changes. It does not record or imply upstream semantic revisions unless an upstream canonical snapshot is explicitly replaced.

## 0.1.0-dev.2 — 2026-08-25

### Added

- repository-side `release_control/PROJECT_SOURCE_CAPACITY_LEDGER.md`
- explicit 20/25 soft-ceiling and 3–5-slot reserve management for Project sources
- retirement-ready classification for initial-tree and intake-verification Project-source copies, without deleting their package history

### Preserved

- all ten foundational/current canonical/support/control owners
- Protocol `v8.3.18`, Trigger `v0.1`, and Regression semantic expectations unchanged
- fresh behavioral deployment status remains unexecuted


## 0.1.0-dev.1 — 2026-08-25

### Added

- public `README.md` entrypoint
- portable `INSTALLATION.md` loading contract
- independent Distribution/upstream version metadata in `VERSION.md`
- release-engineering work-unit record for public entrypoint and metadata gaps
- package-wide SHA-256 inventory

### Preserved

- Protocol `v8.3.18` unchanged
- Trigger Index `v0.1` unchanged
- Regression semantic expectations unchanged
- canonical runtime/support artifact bytes unchanged from intake

### Open release-candidate blockers

- public LICENSE terms / rights holder / redistribution permission are not supplied by the canonical snapshot
- complete CITATION creator/author identity is not supplied by the canonical snapshot
- fresh-environment deployment test has not yet been run for this distribution package

### Deployment-test preparation

- added `tests/fresh_environment/TEST_PLAN.md`
- added `tests/fresh_environment/EXECUTION_RECORD.md`
- static package/source-hash preflight passed
- behavioral fresh-environment execution remains explicitly unperformed
