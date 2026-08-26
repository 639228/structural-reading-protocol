# Work Unit 09 — README Quick-Access Navigation Patch

Status: `PACKAGE MATERIALIZED / VERIFIED / PUBLICATION PENDING`

Distribution: `1.0.3`
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
2. update repository `main` with the verified `1.0.3` README / metadata patch;
3. immediately create tag/release `v1.0.3` targeting that exact `main` commit and attach the verified package assets.

Reason: the `v1.0.3` tag should identify the repository snapshot containing the `1.0.3` public documentation. The `/releases/latest` link may continue to resolve to `v1.0.2` only during the short interval between the main update and release publication.

## Current stop

The `1.0.3` package and repository patch are materialized and verified.

GitHub `main` update and `v1.0.3` tag/release publication remain pending.

`STOP` pending publication.
