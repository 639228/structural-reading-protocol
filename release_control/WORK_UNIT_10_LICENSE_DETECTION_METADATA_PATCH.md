# Work Unit 10 — CC BY 4.0 License Detection / NOTICE Separation / 1.0.4 Recovery

## Required judgment

Can Distribution `1.0.4` be recovered as the intended downstream license-detection / release-metadata patch without changing runtime semantics?

## Classification

`DOWNSTREAM PACKAGING / MATERIALIZATION / PUBLICATION REPAIR`

Not a Protocol or Trigger semantic change.

## Confirmed failure in the first 1.0.4 publication attempt

The first public `v1.0.4` state did not materialize the intended patch coherently:

- the published `v1.0.4` tag pointed to a pre-patch commit;
- `NOTICE.md` and `CITATION.cff` were absent from that tag snapshot;
- root README / README.en / VERSION / CHANGELOG were not fully aligned to the intended `1.0.4` state;
- an invalid two-line third-party package copyright fragment was accidentally installed as root `LICENSE.md` on `main`;
- GitHub therefore continued to report `Other / NOASSERTION` until the root license was corrected;
- the first `v1.0.4` Release had no custom archive/checksum assets.

This is a distribution-side failure. It does not expose a Protocol / Trigger semantic defect.

## Recovery actions completed before republication

1. Replaced root `LICENSE.md` with the full standard Creative Commons Attribution 4.0 International license text.
2. Preserved `NOTICE.md` as the distribution-specific scope / attribution / third-party / no-endorsement supplement.
3. Preserved `CITATION.cff` as machine-readable citation metadata.
4. Aligned Japanese README Distribution/license navigation to `1.0.4`.
5. Aligned English README Distribution/license navigation to `1.0.4`.
6. Aligned root `VERSION.md` and `CHANGELOG.md` to `1.0.4`.
7. Removed temporary root patch-scaffolding files.
8. Re-read GitHub repository metadata: license detection now resolves to `Creative Commons Attribution 4.0 International` / `CC-BY-4.0`.
9. Deleted the malformed first `v1.0.4` Release.
10. Deleted the malformed / pre-patch first `v1.0.4` tag.
11. Preserved Protocol and Trigger canonical hashes.
12. Regenerated package-wide checksums and corrected release assets from the repaired snapshot.

## Fresh behavioral judgment

`NO START`

Reason: no runtime source, runtime ownership, Trigger dispatch, necessity / routing / stop semantics, bootstrap semantics, or minimum runtime pair changes.

## Current publication state

`CORRECTED SNAPSHOT MATERIALIZED / v1.0.4 REPUBLICATION PENDING`

The corrected release must be published only after the release-control files and package checksum inventory are committed to `main`.

## Completion test

After corrected republication, verify:

- tag `v1.0.4` resolves to the corrected release commit;
- tag snapshot contains `NOTICE.md` and `CITATION.cff`;
- tag snapshot contains the full standard CC BY 4.0 `LICENSE.md`;
- README / README.en / VERSION / CHANGELOG are `1.0.4`-consistent;
- release assets contain the corrected archive and checksum sidecar;
- archive checksum matches the sidecar;
- Protocol SHA-256 remains `ea0f05e0b0a87868e92c35a2f4ce38b456fb9980b304c48cf72331a388b618cd`;
- Trigger SHA-256 remains `78f37f241d092c93490301d73396c102f0c248df3f9c48d88302db1e99147146`;
- GitHub repository license metadata remains `CC-BY-4.0`.

Only after these checks may Zenodo archival start.

## Semantic boundary

No Protocol revision, Trigger revision, new runtime operation, new Trigger row, field 4 / field 6 semantic change, Regression expectation change, or Reference Gate change is authorized by this work unit.

Current semantic defect candidate:
`NONE EXPOSED`
