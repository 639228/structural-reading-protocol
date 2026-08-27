# Work Unit 10 — CC BY 4.0 License Detection / NOTICE Separation

## Required judgment

Can the public repository eliminate the GitHub `Other / NOASSERTION` license-surface mismatch without changing runtime semantics?

## Classification

`DOWNSTREAM RELEASE-METADATA / PACKAGING FIX`

Not a Protocol or Trigger semantic change.

## Observed pre-change state

- Repository public metadata reports `license.key=other`, `name=Other`, `spdx_id=NOASSERTION`.
- Root `LICENSE.md` declares CC BY 4.0 but mixes the license decision with project-specific scope, attribution, third-party-material, and no-endorsement explanation.
- Current stable Distribution is `1.0.3`.

## Authorized distribution delta

1. `LICENSE.md` → standard CC BY 4.0 full text only.
2. Add `NOTICE.md` containing distribution-specific scope / attribution / third-party / no-endorsement guidance.
3. Update README navigation to point separately to LICENSE, NOTICE, and CITATION.
4. Distribution → `1.0.4`.
5. Regenerate package-wide checksums/archive if a full successor package is materialized.

## Fresh behavioral judgment

`NO START`

Reason: no runtime source, runtime ownership, Trigger dispatch, necessity/route/stop semantics, bootstrap semantics, or minimum runtime pair changes.

## Completion test

After publishing the successor repository/package state, re-read GitHub repository metadata. Desired observed state:

- license name: `Creative Commons Attribution 4.0 International`
- SPDX: `CC-BY-4.0`

If GitHub remains `Other / NOASSERTION`, record that as a hosting/license-detection issue; do not infer a semantic defect.

## Current execution limitation

The connected GitHub integration returned HTTP 403 for branch creation and file update, so this session could not publish the patch. The patch bundle is prepared locally for application.
