# Current Release Readiness State

State revision: `1.15`

Status: `DISTRIBUTION_1.0.5_DOI_METADATA_PATCH_MATERIALIZED / PUBLICATION_PENDING`

Distribution: `1.0.5`

Stable predecessor: `1.0.4`

Canonical handoff: `PUBLIC_DISTRIBUTION_CANONICAL_SNAPSHOT_V1.0`

Upstream semantic identity:
- Protocol `v8.3.18`
- Trigger Index `v0.1`

Public repository:
- `https://github.com/639228/structural-reading-protocol`

## 1. Role

This is the downstream pre-publication readiness state for Distribution `1.0.5`.

It supersedes revision `1.14` as current downstream release-control owner only after this file is actually admitted as the Project-backed current source.

It is not a semantic owner and does not replace the Protocol, Trigger Index, canonical handoff, developer/research owners, evidence/provenance owners, GitHub live public state, or Zenodo live public state.

## 2. Predecessor closure

Distribution `1.0.4` remains:

`GITHUB PUBLISHED / VERIFIED / ZENODO PUBLISHED / DOI ASSIGNED / CLOSED`

Its published tag, GitHub Release, archive, Zenodo version record, and DOI are immutable predecessors for this work unit.

No `1.0.4` publication artifact is rewritten by Distribution `1.0.5`.

## 3. DOI state for successor

Distribution `1.0.5` version DOI:

`10.5281/zenodo.22129037`

All-versions / concept DOI:

`10.5281/zenodo.22127380`

Current `1.0.5` DOI state at this readiness point:

`RESERVED / NOT YET REGISTERED`

The version DOI was reserved in a Zenodo `New version` draft derived from the published `1.0.4` version chain.

Publication / registration remains pending until the `1.0.5` Zenodo record is actually published and verified.

## 4. Distribution delta

Distribution `1.0.5` changes downstream bibliographic/release metadata only:

- `README.md`
- `README.en.md`
- `CITATION.md`
- `CITATION.cff`
- `VERSION.md`
- `CHANGELOG.md`
- `release_control/CURRENT_RELEASE_READINESS_STATE.md`
- regenerated `release_control/PACKAGE_SHA256SUMS.txt`

No runtime artifact is changed.

## 5. Runtime / support preservation

Canonical Protocol SHA-256:

`ea0f05e0b0a87868e92c35a2f4ce38b456fb9980b304c48cf72331a388b618cd`

Canonical Trigger SHA-256:

`78f37f241d092c93490301d73396c102f0c248df3f9c48d88302db1e99147146`

Support identities remain:

- Coverage `v0.8`
- Manifest `v0.8`
- Retrieval `v1.9`
- Regression `v1.2`
- Cross `v0.20`
- Integration `v0.11`

Current semantic defect candidate:

`NONE EXPOSED`

## 6. Fresh behavioral judgment

New fresh behavioral run:

`NO START`

Reason:

The actual `1.0.5` delta is DOI / citation / README / version / release-control metadata only. It does not alter runtime loading, bootstrap, source selection, dispatch, semantic ownership, minimum runtime composition, installation behavior, Protocol bytes, or Trigger bytes.

Saved bounded fresh-environment evidence remains at its previously recorded strength only.

## 7. Materialization verification

Expected package file count:

`39`

Expected changed files relative to the published `1.0.4` package:

`8`

The two checksum inventories are not self-hashed; `PACKAGE_SHA256SUMS.txt` records the other 38 package files.

Required materialization checks:

- package file count = 39;
- changed-file set exactly matches the downstream metadata delta plus regenerated package checksum inventory;
- Protocol / Trigger canonical SHA-256 unchanged;
- current support-owner SHA-256 unchanged;
- deterministic archive regeneration;
- archive re-extraction byte-for-byte match.

These checks must pass before publication.

## 8. Publication gate

GitHub `v1.0.5` tag:

`NOT YET PUBLISHED`

GitHub Release `v1.0.5`:

`NOT YET PUBLISHED`

Zenodo `1.0.5` record:

`DRAFT / DOI RESERVED`

Zenodo DOI registration:

`NOT YET REGISTERED`

Do not report any of these later publication states as complete before live verification.

Before publishing the GitHub Release, ensure Zenodo GitHub automatic preservation for this repository is disabled so the manually maintained Zenodo version chain is not unintentionally duplicated.

## 9. Semantic boundary

No current observation authorizes:

- Protocol semantic revision;
- Trigger semantic revision;
- a new runtime operation;
- a new Trigger row;
- field 4 / field 6 semantic change;
- Regression expectation change;
- Reference Gate repair.

Current semantic defect candidate:

`NONE EXPOSED`

## 10. Current judgment

Distribution `1.0.5` materialization:

`READY FOR VERIFICATION`

GitHub publication:

`PENDING`

Zenodo publication:

`PENDING`

DOI:

`RESERVED / NOT YET REGISTERED`

Protocol:

`v8.3.18` unchanged

Trigger Index:

`v0.1` unchanged
