# Current Release Readiness State

State revision: `1.13`

Status: `DISTRIBUTION_1.0.4_PUBLISHED_VERIFIED / CURRENT_RELEASE_WORK_UNIT_CLOSED`

Distribution: `1.0.4`

Stable predecessor: `1.0.3`

Canonical handoff: `PUBLIC_DISTRIBUTION_CANONICAL_SNAPSHOT_V1.0`

Upstream semantic identity:
- Protocol `v8.3.18`
- Trigger Index `v0.1`

Public repository:
- `https://github.com/639228/structural-reading-protocol`

## 1. Role

This is the downstream post-publication closure state for corrected Distribution `1.0.4`.

It closes the downstream recovery work for the incomplete / malformed first `1.0.4` publication attempt after verifying the corrected GitHub tag, Release, release assets, license detection, package identity, and runtime preservation.

This closure does not revise Protocol semantics, Trigger runtime semantics, Regression expectations, upstream canonical source selection, or saved behavioral evidence strength.

The published `v1.0.4` tag remains the immutable corrected release snapshot. This post-publication closure is recorded after publication and does not move or rewrite that tag.

## 2. Distribution delta

Distribution `1.0.4` is a downstream license-detection / release-metadata packaging patch over published stable `1.0.3`.

The corrected delta is limited to:

- standard Creative Commons Attribution 4.0 International license text in root `LICENSE.md`;
- distribution-specific scope / attribution / third-party-material / no-endorsement guidance in `NOTICE.md`;
- machine-readable `CITATION.cff`;
- Japanese and English README license navigation and Distribution metadata;
- root `VERSION.md` and `CHANGELOG.md` alignment to `1.0.4`;
- release-control recovery record and regenerated package checksum inventory;
- corrected release archive materialization and republication.

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

Reason: the `1.0.4` repair changes license / NOTICE / citation / version metadata, release-control state, and packaging only. It does not change runtime ownership, Trigger necessity / routing / stop semantics, bootstrap semantics, or the minimum runtime pair.

Saved fresh evidence remains `8 / 8 PREPARED FD CASES PASS` at its existing bounded strength only.

This does not establish protocol-wide adequacy, natural whole-protocol execution, cross-model / cross-environment reproducibility, absence of systematic weakness, historical firstness / absence of prior art, universal performance improvement, or language equivalence.

## 4. Corrected GitHub publication verification

Publication status:
`PASS`

Verified public release:

- tag: `v1.0.4`;
- tag target commit: `ee2544504c860c5a9a2cb5314309f73f75f9425b`;
- Release title: `構造的読解プロトコル — Public Distribution 1.0.4`;
- Release state: published;
- draft: `false`;
- prerelease: `false`;
- Latest Release: `v1.0.4`;
- published at: `2026-08-27T04:37:49Z`.

Verified release assets:

1. `public_distribution_1.0.4.tar.gz`
   - SHA-256: `be882cfa2cbff6fed18bda0b44042081f683b3bda38211e4a5a70c6e3acf304c`

2. `public_distribution_1.0.4.tar.gz.sha256`
   - GitHub asset digest: `sha256:1d0962335811cc39c53602391d7d2c66bacd1af75f07b081579fd8012af1cb6f`

The uploaded archive digest matches the expected corrected release archive digest.

GitHub repository license detection:

- name: `Creative Commons Attribution 4.0 International`;
- SPDX: `CC-BY-4.0`;
- status: `PASS`.

## 5. Runtime preservation verification

Runtime semantic identity remains unchanged.

Canonical SHA-256:

- Protocol `v8.3.18`:
  `ea0f05e0b0a87868e92c35a2f4ce38b456fb9980b304c48cf72331a388b618cd`

- Trigger Index `v0.1`:
  `78f37f241d092c93490301d73396c102f0c248df3f9c48d88302db1e99147146`

GitHub blob SHA at published tag `v1.0.4`:

- Protocol:
  `bca89a7e61bda583fa34d6bc66b7dc57f2739c7d`

- Trigger Index:
  `e6e2ee051b605bcc4436f4d58288665a385c6ecc`

The Git blob identifiers and canonical SHA-256 values are different hash systems and are recorded separately. No runtime source rewrite is inferred from their difference.

The published tag checksum inventory records the canonical Protocol and Trigger SHA-256 values unchanged.

## 6. Package verification

Materialization status:
`PASS`

Verified corrected release materialization:

- package file count: `39`;
- package-wide checksum inventory regenerated for the corrected release snapshot;
- Protocol and Trigger canonical SHA-256 preserved;
- current semantic/support owner hashes preserved;
- release archive regenerated from the corrected snapshot;
- archive re-extraction and byte-for-byte comparison passed before upload;
- uploaded archive digest matches the verified local archive digest;
- no semantic source rewrite is part of this materialization.

## 7. Work-unit closure

Work Unit 10 status:
`CLOSED`

Resolved downstream failures:

- malformed first `LICENSE.md` materialization;
- incomplete root application of the intended `1.0.4` patch;
- pre-patch first `v1.0.4` tag;
- first Release with zero custom assets;
- stale README / README.en / VERSION / CHANGELOG state;
- temporary root patch-scaffolding files;
- stale `Other / NOASSERTION` GitHub license detection;
- stale pre-publication release-control state at the time corrected publication work began.

No current observation exposes a Protocol / Trigger semantic defect.

Current semantic defect candidate:
`NONE EXPOSED`

## 8. Zenodo gate

GitHub publication prerequisite:
`SATISFIED`

Zenodo:
`START AUTHORIZED`

Reason:

- corrected `v1.0.4` publication is complete;
- tag identity is verified;
- release assets are verified;
- archive digest is verified;
- repository license detection is verified;
- canonical runtime identity is preserved.

The next downstream publication objective may therefore be Zenodo archival and DOI acquisition.

If a DOI is later incorporated into repository documentation or a newly published package, that should be handled as a later Distribution metadata patch rather than by rewriting the published `v1.0.4` tag.

## 9. Semantic boundary

No current observation authorizes:

- Protocol semantic revision;
- Trigger semantic revision;
- a new runtime operation;
- a new Trigger row;
- field 4 / field 6 semantic change;
- Regression expectation change;
- Reference Gate repair;
- any claim of protocol-wide adequacy;
- any claim of natural whole-protocol execution;
- any claim of cross-model / cross-environment reproducibility;
- any claim of absence of systematic weakness;
- any claim of historical firstness / absence of prior art;
- any claim of universal performance improvement.

Current semantic defect candidate:
`NONE EXPOSED`

## 10. Current downstream judgment

Distribution `1.0.4`:
`PUBLISHED / VERIFIED / CLOSED`

GitHub release-control closure:
`PASS`

Zenodo:
`START AUTHORIZED`

Protocol:
`v8.3.18` unchanged

Trigger Index:
`v0.1` unchanged
