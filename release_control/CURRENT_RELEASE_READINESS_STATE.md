# Current Release Readiness State

State revision: `1.12`

Status: `CORRECTED_1.0.4_MATERIALIZED / RELEASE_REPUBLICATION_PENDING`

Distribution: `1.0.4`

Stable predecessor: `1.0.3`

Canonical handoff: `PUBLIC_DISTRIBUTION_CANONICAL_SNAPSHOT_V1.0`

Upstream semantic identity:
- Protocol `v8.3.18`
- Trigger Index `v0.1`

Public repository:
- `https://github.com/639228/structural-reading-protocol`

## 1. Role

This is the downstream pre-publication state for the corrected Distribution `1.0.4` snapshot.

It records repair of an incomplete / malformed first `1.0.4` publication attempt. The repair is limited to distribution packaging, license/citation metadata, public documentation/version alignment, release-control state, and release materialization.

It does not revise Protocol semantics, Trigger runtime semantics, Regression expectations, upstream canonical source selection, or saved behavioral evidence strength.

## 2. Corrected distribution delta

The corrected `1.0.4` delta is limited to:

- standard Creative Commons Attribution 4.0 International license text in root `LICENSE.md`;
- distribution-specific scope / attribution / third-party-material / no-endorsement guidance in `NOTICE.md`;
- machine-readable `CITATION.cff`;
- Japanese and English README license navigation and Distribution metadata;
- root `VERSION.md` and `CHANGELOG.md` alignment to `1.0.4`;
- release-control repair record and regenerated package checksum inventory;
- corrected release archive materialization.

Unchanged semantic/support identity:

- Protocol `v8.3.18`;
- Trigger Index `v0.1`;
- Coverage `v0.8`;
- Manifest `v0.8`;
- Retrieval `v1.9`;
- Regression `v1.2`;
- Cross `v0.20`;
- Integration `v0.11`.

## 3. Fresh behavioral judgment

New run:
`NO START`

Reason: the repair does not change runtime ownership, Trigger necessity / routing / stop semantics, bootstrap semantics, or the minimum runtime pair.

Saved fresh evidence remains `8 / 8 PREPARED FD CASES PASS` at its existing bounded strength only.

This does not establish protocol-wide adequacy, natural whole-protocol execution, cross-model / cross-environment reproducibility, absence of systematic weakness, historical firstness / absence of prior art, or universal performance improvement.

## 4. Recovered publication state before corrected release

Observed after root repair and before corrected `v1.0.4` republication:

- root README / README.en / VERSION / CHANGELOG aligned to Distribution `1.0.4`;
- full standard CC BY 4.0 license text present in root `LICENSE.md`;
- `NOTICE.md` present;
- `CITATION.cff` present with `version: 1.0.4` and `license: CC-BY-4.0`;
- temporary root patch-scaffolding files removed;
- GitHub repository license metadata resolves to `Creative Commons Attribution 4.0 International` / `CC-BY-4.0`;
- malformed first `v1.0.4` Release deleted;
- malformed / pre-patch first `v1.0.4` tag deleted.

The corrected `v1.0.4` tag and Release are not yet republished at this state revision.

## 5. Package verification

Materialization status:
`PASS`

Verified for the corrected release materialization:

- package file count: `39`;
- Protocol SHA-256 preserved: `ea0f05e0b0a87868e92c35a2f4ce38b456fb9980b304c48cf72331a388b618cd`;
- Trigger SHA-256 preserved: `78f37f241d092c93490301d73396c102f0c248df3f9c48d88302db1e99147146`;
- current semantic/support owner hashes preserved;
- package-wide checksum inventory regenerated from the corrected snapshot;
- release archive regenerated from the corrected snapshot;
- archive re-extraction and byte-for-byte file comparison required to pass before upload;
- no semantic source rewrite is part of this materialization.

## 6. Publication gate

Publication status:
`PENDING`

Before Zenodo, verify after republication:

- new tag `v1.0.4` points to the corrected release commit;
- tag snapshot contains the corrected 39-file distribution state;
- GitHub Release title identifies Public Distribution `1.0.4`;
- release assets include `public_distribution_1.0.4.tar.gz` and `public_distribution_1.0.4.tar.gz.sha256`;
- uploaded archive digest equals the sidecar digest;
- GitHub license metadata remains `CC-BY-4.0`;
- Protocol and Trigger identities remain unchanged.

Zenodo:
`NO START` until corrected GitHub `v1.0.4` publication is verified.

## 7. Semantic boundary

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
