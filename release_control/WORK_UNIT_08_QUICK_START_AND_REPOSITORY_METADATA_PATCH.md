# Work Unit 08 — Public Entrypoint / ChatGPT Setup / Repository Metadata Patch

Status: `PUBLISHED / VERIFIED / CLOSED`

Distribution: `1.0.2`

Stable predecessor: `1.0.1`

Canonical semantic identity:
- Protocol `v8.3.18`
- Trigger Index `v0.1`

Public repository:
- `https://github.com/639228/structural-reading-protocol`

## Purpose

Integrate the public-facing README selected for release, make ChatGPT setup understandable from the Japanese UI, preserve the already tested four-file first-time loading path, add English navigation/loading documents, record the assigned repository metadata, and publish the verified distribution without changing canonical semantics.

This is downstream distribution/documentation work. It does not revise upstream canonical semantics.

## Distribution delta

User-facing documentation changes:
- `README.md`: adopt the problem-first public entrypoint explaining what execution-control problem the Protocol addresses, what it can do, why it can be useful, concrete uses, and detailed ChatGPT setup;
- `INSTALLATION.md`: Japanese installation guide using ChatGPT's Japanese UI term `情報源`;
- `README.en.md`: English distribution/navigation guide; explicitly not a translated canonical runtime;
- `INSTALLATION.en.md`: English loading guide; explicitly not a translated canonical runtime;
- first-time recommended ChatGPT Project input: README + INSTALLATION + Protocol + Trigger Index;
- minimum runtime remains Protocol + Trigger Index;
- `CITATION.md` / `VERSION.md`: assigned repository metadata retained;
- `CHANGELOG.md`: record this patch.

Release-control changes:
- update `release_control/CURRENT_RELEASE_READINESS_STATE.md`;
- keep `release_control/PROJECT_SOURCE_CAPACITY_LEDGER.md` at its already observed state;
- close this Work Unit 08 after publication verification;
- preserve the released tag as the release snapshot while allowing later administrative closure records on `main`.

## Runtime / semantic boundary

The public documents explain existing canonical behavior. They do not own or revise it.

The canonical runtime pair remains:
- `runtime/構造的読解プロトコル v8.3.18.txt`;
- `runtime/Trigger_Index_candidate_v0.1.txt`.

The Trigger Index remains runtime dispatch rather than a fixed checklist. Candidate existence is not START. Valid `NO START`, `NO FIRE`, and `STOP` outcomes are preserved.

The English documents are navigation/loading documents only. No English canonical Protocol or Trigger is created or claimed.

## Fresh behavioral judgment

New run: `NO START`.

Reason: the revised first-time recommendation uses the same four public inputs already used by the saved fresh-environment deployment test (README, INSTALLATION, Protocol, Trigger), while the canonical runtime pair and bootstrap role separation are unchanged in semantic ownership. The public explanation does not add a semantic operation or change Trigger necessity/route/stop conditions.

The saved evidence remains bounded at its recorded strength.

## Materialization verification

Result:
`PASS`

Verified before publication:
- runtime Protocol and Trigger hashes match `SOURCE_SHA256SUMS.txt`;
- preserved canonical support payloads remain byte-identical to verified `1.0.1`;
- `README.en.md` and `INSTALLATION.en.md` are present in the archive;
- Japanese/English loading guidance agrees on first-time four-file setup vs two-file minimum runtime;
- package-wide SHA-256 inventory passes;
- rebuilt archive re-extracts successfully;
- no symlinks are present.

## Publication verification

Result:
`PASS`

Verified:
- `v1.0.2` Release exists and is public;
- it is not a draft and not a prerelease;
- it is the current Latest Release;
- `v1.0.2` tag points to commit `eef49226b8f9d251b8f662e6491c535ebc530e6f`;
- `public_distribution_1.0.2.tar.gz` is attached;
- published archive SHA-256 is `881aba5ccfba4787dc01734050a3c8690d5ab79a72973313ea6dc79207f70434`;
- Release body declares the same archive SHA-256;
- checksum sidecar is attached;
- `v1.0.1` historical Release is restored;
- `v1.0.1` tag points to `f9719b32fbbfe9e119fd68bb72164f76e922763f`;
- `v1.0.1` archive SHA-256 remains `7b1d0db2711fdc3e0b622d813068072fc86de55d23cebaabb94ee1008038e42d`.

## Result

`PASS_STABLE_DOCUMENTATION_PATCH_1.0.2_PUBLICATION`

The public-entrypoint and loading-documentation changes are published at downstream distribution strength only. No canonical semantic or evidence-strength claim is upgraded.

## Stop

Work Unit 08 is closed.

Further behavioral testing: `NO START`.

Semantic patching: `NO START`.

Further publication work: `NO START` absent a concrete distribution defect, metadata correction, asset-integrity failure, or successor release requirement.

`STOP`
