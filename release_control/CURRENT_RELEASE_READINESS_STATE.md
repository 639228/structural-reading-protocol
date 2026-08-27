# Current Release Readiness State

State revision: `1.14`

Status: `DISTRIBUTION_1.0.4_GITHUB_AND_ZENODO_PUBLISHED_VERIFIED / DOI_ASSIGNED / CURRENT_RELEASE_WORK_UNIT_CLOSED`

Distribution: `1.0.4`

Stable predecessor: `1.0.3`

Canonical handoff: `PUBLIC_DISTRIBUTION_CANONICAL_SNAPSHOT_V1.0`

Upstream semantic identity:
- Protocol `v8.3.18`
- Trigger Index `v0.1`

Public repository:
- `https://github.com/639228/structural-reading-protocol`

## 1. Role

This is the downstream post-Zenodo publication closure state for Distribution `1.0.4`.

It supersedes readiness revision `1.13` as the current downstream release-control owner after successful Zenodo publication and DOI assignment.

This file is not a semantic owner and does not replace the Protocol, Trigger Index, canonical handoff, developer/research owners, evidence/provenance owners, GitHub public state, or Zenodo public record.

## 2. GitHub publication state

GitHub Distribution `1.0.4` remains:

`PUBLISHED / VERIFIED / CLOSED`

Verified release identity retained from revision `1.13`:

- tag: `v1.0.4`
- corrected tag target commit: `ee2544504c860c5a9a2cb5314309f73f75f9425b`
- release archive: `public_distribution_1.0.4.tar.gz`
- archive SHA-256: `be882cfa2cbff6fed18bda0b44042081f683b3bda38211e4a5a70c6e3acf304c`
- checksum sidecar present
- GitHub license detection: `Creative Commons Attribution 4.0 International / CC-BY-4.0`

The published `v1.0.4` tag is not moved or rewritten by this closure.

## 3. Zenodo publication closure

Zenodo state:

`PUBLISHED / VERIFIED AT RECORD-PAGE LEVEL`

Public record:

- record ID: `22127381`
- record URL: `https://zenodo.org/records/22127381`
- resource type: `Software`
- Distribution version: `1.0.4`
- publication date: `2026-08-27`
- creator: `639228`
- access: open / public

Published file:

- `public_distribution_1.0.4.tar.gz`
- Zenodo-displayed MD5: `a360c82de434f7f2f1f3b30f5b3f5168`
- corresponding verified GitHub/local SHA-256:
  `be882cfa2cbff6fed18bda0b44042081f683b3bda38211e4a5a70c6e3acf304c`

The Zenodo file therefore preserves the verified corrected Distribution `1.0.4` archive identity.

## 4. DOI state

Version DOI:

`10.5281/zenodo.22127381`

All-versions / concept DOI:

`10.5281/zenodo.22127380`

Zenodo publication state is no longer a reserved-draft state.

Zenodo's documented DOI behavior registers the DOI when the record is published. The published record displays the version DOI and the all-versions DOI.

DOI state:

`ASSIGNED / PUBLISHED`

No DOI was inserted retroactively into the already-published GitHub `v1.0.4` tag or release archive.

## 5. Zenodo metadata state

Main title:

`構造的読解プロトコル — Public Distribution 1.0.4`

Translated title:

`Structural Reading Protocol — Public Distribution 1.0.4`

English subtitle:

`A Natural-Language Execution Architecture for LLM Reading, Inquiry, Research, and Evaluation`

License:

`Creative Commons Attribution 4.0 International (CC BY 4.0)`

Keywords / subjects recorded:

- `large language models`
- `LLM`
- `ChatGPT`
- `close reading`
- `reasoning`
- `natural language programming`
- `natural language execution architecture`
- `runtime dispatch`
- `inquiry`
- `research`
- `evaluation`

These metadata describe the existing public distribution and do not revise canonical runtime semantics.

## 6. Runtime / semantic preservation

Protocol:

`v8.3.18` unchanged

Canonical Protocol SHA-256:

`ea0f05e0b0a87868e92c35a2f4ce38b456fb9980b304c48cf72331a388b618cd`

Trigger Index:

`v0.1` unchanged

Canonical Trigger SHA-256:

`78f37f241d092c93490301d73396c102f0c248df3f9c48d88302db1e99147146`

Support identity remains:

- Coverage `v0.8`
- Manifest `v0.8`
- Retrieval `v1.9`
- Regression `v1.2`
- Cross `v0.20`
- Integration `v0.11`

Current semantic defect candidate:

`NONE EXPOSED`

## 7. Fresh behavioral judgment

New fresh behavioral run for Zenodo archival / DOI assignment:

`NO START`

Reason:

Zenodo publication used the already-verified Distribution `1.0.4` archive and added repository metadata / DOI state only. Runtime loading, bootstrap, minimum runtime composition, semantic ownership, Trigger dispatch semantics, and canonical runtime bytes were not changed.

Saved bounded fresh-environment evidence remains at its previously recorded strength only.

## 8. Work-unit closure

GitHub corrected `1.0.4` publication work:

`CLOSED`

Zenodo repository enablement / manual archival / DOI acquisition work:

`CLOSED`

Distribution `1.0.4` archival state:

`GITHUB PUBLISHED / ZENODO PUBLISHED / DOI ASSIGNED`

No semantic repair is authorized.

## 9. Newly exposed downstream metadata delta

After Zenodo publication, current GitHub `main` still contains pre-DOI metadata in at least:

- `CITATION.md`: DOI `not yet assigned`
- `VERSION.md`: DOI `not yet assigned`
- `CITATION.cff`: no DOI field for the newly assigned Zenodo DOI

This is downstream bibliographic metadata staleness, not a semantic defect and not a defect in the immutable `v1.0.4` release snapshot.

The published `v1.0.4` tag must not be rewritten merely to add DOI metadata.

## 10. Next work unit

Next concrete Release Engineering work unit:

`Distribution 1.0.5 — DOI metadata patch`

Start judgment:

`START`

Reason:

A DOI now exists while current repository bibliographic/version metadata still represents the pre-DOI state. A successor Distribution is the correct place to formally propagate the DOI without mutating the published `v1.0.4` tag.

Expected change class:

- citation / bibliographic metadata
- documentation metadata
- release-control metadata
- Distribution version metadata

Expected semantic effect:

`NONE`

Expected Protocol version:

`v8.3.18` unchanged

Expected Trigger Index version:

`v0.1` unchanged

Expected fresh behavioral rerun judgment:

`NO START`, unless the actual `1.0.5` patch changes runtime loading, bootstrap, source selection, dispatch, semantic ownership, minimum runtime composition, or installation behavior.

## 11. Current downstream judgment

Distribution `1.0.4`:

`PUBLISHED / VERIFIED / ARCHIVED / DOI ASSIGNED / CLOSED`

GitHub:

`PASS`

Zenodo:

`PASS`

Version DOI:

`10.5281/zenodo.22127381`

Concept DOI:

`10.5281/zenodo.22127380`

Current release-control owner:

`revision 1.14` once Project-backed

Next work unit:

`Distribution 1.0.5 — DOI metadata patch / START`
