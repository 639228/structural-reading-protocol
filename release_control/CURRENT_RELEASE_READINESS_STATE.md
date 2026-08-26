# Current Release Readiness State

State revision: `1.10`

Status: `STABLE_DOCUMENTATION_PATCH_MATERIALIZED / PUBLICATION_PENDING`

Distribution: `1.0.3`

Stable predecessor: `1.0.2`

Canonical handoff: `PUBLIC_DISTRIBUTION_CANONICAL_SNAPSHOT_V1.0`

Upstream semantic identity:
- Protocol `v8.3.18`
- Trigger Index `v0.1`

Current Project-backed predecessor:
- `CURRENT_RELEASE_READINESS_STATE_v1.9(1).md`

Public repository:
- `https://github.com/639228/structural-reading-protocol`

## 1. Role

This is the downstream release-state successor candidate for Distribution `1.0.3`, a README quick-access/navigation documentation patch over published stable `1.0.2`.

It does not revise canonical Protocol semantics, Trigger runtime semantics, Regression expectations, upstream source selection, or saved behavioral evidence strength.

## 2. Distribution delta

The `1.0.3` delta is limited to public navigation / distribution metadata:
- add top-level `English / Installation / Latest Release` navigation in the Japanese primary README;
- add a compact `最短で試す` section after the opening problem statement and before `これは何か`;
- preserve the established first-time four-file ChatGPT setup;
- preserve Protocol + Trigger as the minimum runtime pair;
- use repository-relative `INSTALLATION.md` rather than a ChatGPT-internal Project/conversation URL;
- update Distribution metadata and changelog to `1.0.3`.

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

New run: `NO START`.

Reason: the patch only shortens navigation to the already documented four-file loading path and existing bootstrap instructions. It does not change runtime ownership, Trigger necessity/route/stop semantics, or the minimum runtime pair.

Saved fresh evidence remains `8 / 8 PREPARED FD CASES PASS` at its existing bounded strength only.

## 4. Package verification

Materialization status: `PASS`.

Required checks:
- verified `1.0.1` stable archive used as physical semantic/support base;
- verified final `1.0.2` repository patch SHA-256 `78d1a303601498dd01d6bd6113f0fecdffae6462d1dbac0424d30542add13ffc` applied;
- post-publication `1.0.2` closure control patch applied;
- accepted `1.0.3` README/navigation patch applied;
- canonical/source SHA-256 inventory preserved;
- package-wide checksum inventory regenerated and verified;
- archive re-extraction verified;
- no symlinks present.

## 5. Publication state

`v1.0.3` GitHub publication: `PENDING`.

Preferred sequence:
1. update `main` with the verified `1.0.3` repository patch;
2. immediately create `v1.0.3` targeting that exact commit;
3. attach the verified `1.0.3` archive and checksum sidecar;
4. verify tag target, Latest status, and asset digest;
5. only then close publication state.

The published `v1.0.2` release remains unchanged until `v1.0.3` is actually published.

## 6. Semantic boundary

No current observation authorizes Protocol revision, Trigger revision, new runtime operation, new Trigger row, field 4/6 semantic change, Regression expectation change, Reference Gate repair, or translated canonical runtime promotion.

Current semantic defect candidate: `NONE EXPOSED`.

## 7. Project-source admission

The current Project-backed readiness owner remains `CURRENT_RELEASE_READINESS_STATE_v1.9(1).md` until this successor state is explicitly admitted.

This `1.10` artifact is a successor candidate only at the present pre-publication stage.

## 8. Stop condition

Package materialization and verification are complete.

Further behavioral testing: `NO START`.

Semantic patching: `NO START`.

Next required downstream work: GitHub `main` update and `v1.0.3` publication verification.

At current inputs: `STOP` pending publication.

END
