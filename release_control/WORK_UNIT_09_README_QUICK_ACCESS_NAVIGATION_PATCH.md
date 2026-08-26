# Work Unit 09 — README Quick-Access Navigation Patch

Status: `CANDIDATE MATERIALIZED / PACKAGE NOT YET MATERIALIZED`

Distribution candidate: `1.0.3`
Stable predecessor: `1.0.2`

Canonical semantic identity:
- Protocol `v8.3.18`
- Trigger Index `v0.1`

## Scope

Downstream documentation/navigation only:

- add top README links for English / Installation / Latest Release;
- add a compact `最短で試す` section between the opening problem statement and `これは何か`;
- preserve the already established first-time four-file setup;
- preserve Protocol + Trigger as the minimum runtime pair;
- use repository-relative `INSTALLATION.md`, not a ChatGPT-internal URL.

No Protocol, Trigger, Regression, Coverage, Manifest, Retrieval, Cross, Integration, license, or evidence semantic change is authorized.

## Behavioral judgment

Fresh rerun: `NO START`.

Reason: the patch does not change loading semantics or runtime ownership. It only shortens navigation to the existing 4-file setup and existing bootstrap instructions.

## Publication order

Preferred publication sequence:

1. materialize and verify the `1.0.3` package;
2. publish GitHub Release `v1.0.3` with the verified package assets;
3. update repository `main` with the `1.0.3` README / metadata patch in the same publication work unit or immediately after release publication.

Reason: the README top navigation uses `/releases/latest`; until `v1.0.3` is published, that link correctly resolves to the currently published `v1.0.2`.

## Current stop

README/repository patch candidate is materialized and internally version-consistent.

Package/archive materialization and GitHub `v1.0.3` publication are separate later steps.

`STOP` pending package materialization.
