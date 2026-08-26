# Work Unit 08 — Public Entrypoint / ChatGPT Setup / Repository Metadata Patch

Status: `MATERIALIZED / VERIFIED / PUBLICATION_UPDATE_PENDING`

Distribution: `1.0.2`

Stable predecessor: `1.0.1`

Canonical semantic identity:
- Protocol `v8.3.18`
- Trigger Index `v0.1`

Public repository:
- `https://github.com/639228/structural-reading-protocol`

## Purpose

Integrate the public-facing README selected for release, make ChatGPT setup understandable from the Japanese UI, preserve the already tested four-file first-time loading path, add English navigation/loading documents, and record the assigned repository metadata.

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
- update this Work Unit 08;
- regenerate `release_control/PACKAGE_SHA256SUMS.txt`.

## Runtime / semantic boundary

The public documents explain existing canonical behavior. They do not own or revise it.

The canonical runtime pair remains:
- `runtime/構造的読解プロトコル v8.3.18.txt`;
- `runtime/Trigger_Index_candidate_v0.1.txt`.

The Trigger Index remains runtime dispatch rather than a fixed checklist. Candidate existence is not START. Valid `NO START`, `NO FIRE`, and `STOP` outcomes are preserved.

The English documents are navigation/loading documents only. No English canonical Protocol or Trigger is created or claimed.

## Fresh behavioral judgment

New run: `NO START`.

Reason: the revised first-time recommendation uses the same four public inputs already used by the saved fresh-environment deployment test (README, INSTALLATION, Protocol, Trigger), while the canonical runtime pair and bootstrap role separation are unchanged in semantic ownership. The new public explanation does not add a semantic operation or change Trigger necessity/route/stop conditions.

The saved evidence remains bounded at its recorded strength.

## Verification requirement

Before closure:
- runtime Protocol and Trigger hashes must match `SOURCE_SHA256SUMS.txt`;
- canonical support payloads must remain byte-identical to verified `1.0.1`;
- new English documents must actually be present in the archive;
- Japanese/English loading guidance must agree on first-time four-file setup vs two-file minimum runtime;
- package-wide SHA-256 inventory must PASS;
- rebuilt archive must re-extract successfully;
- no symlinks may be present.

## Result

`PASS_STABLE_DOCUMENTATION_PATCH_1.0.2_MATERIALIZATION`

The public-entrypoint and loading-documentation changes are integrated at downstream distribution strength only. No canonical semantic or evidence-strength claim is upgraded.
