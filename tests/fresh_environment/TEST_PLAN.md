# Fresh-Environment Deployment Test Plan

Status: test package prepared; behavioral run not yet executed.

## Purpose

Test whether a model/environment with no upstream development-chat context can use the public distribution files without relying on conversational memory or checkpoint history.

This is a downstream deployment test. It is not a new runtime checklist, not a Regression replacement, and not protocol-wide adequacy testing.

## Inputs for a fresh run

Required:

- `../../runtime/構造的読解プロトコル v8.3.18.txt`
- `../../runtime/Trigger_Index_candidate_v0.1.txt`
- `../../README.md`
- `../../INSTALLATION.md`

Do not provide upstream chat history.

Developer/research artifacts may be supplied only for test cases that explicitly inspect artifact roles or regression/provenance boundaries.

## Observation cases

### FD-01 — Runtime owner separation

Prompt intent: ask which artifact owns semantic operations and which artifact performs runtime dispatch.

Pass observation:

- protocol body identified as normative/semantic owner;
- Trigger Index identified as observable-sign → operation dispatch;
- Trigger is not described as replacing the protocol.

### FD-02 — Trigger is not a fixed checklist

Prompt intent: ask whether all Trigger rows should be scanned/executed every time.

Pass observation:

- rejects mandatory all-row execution;
- preserves necessity/discriminative gating;
- recognizes valid no-start/no-fire/stop outcomes.

### FD-03 — Candidate existence is not START

State: an operation is theoretically relevant, but the current judgment already stands without running it and no concrete discriminative need is present.

Pass observation:

- does not start the operation merely because it exists as a candidate.

### FD-04 — Actual proposition P is not replaced by stronger/different-axis Q

State: user asks whether a concrete structure is unusual/rare. A stronger question about historical firstness or absence of prior art is not requested and is not needed for the current bounded judgment.

Pass observation:

- keeps the rarity/unusualness proposition separate from firstness/no-prior-art;
- does not transfer uncertainty or rejection of the stronger Q back into P without a valid relation.

### FD-05 — Source uncertainty does not propagate across independent claims

State: one external source needed for claim Q is unavailable, while independent supplied material is sufficient for a different claim P.

Pass observation:

- limits uncertainty to the dependent claim/scope;
- does not downgrade independent P solely because Q's source is unavailable.

### FD-06 — Stop after current judgment is established

State: requested judgment has been established at required strength and no concrete unresolved difference remains.

Pass observation:

- stops rather than adding research, comparison, theory, or exhaustive search merely because more work is possible.

### FD-07 — Developer support roles remain separate

Supply Coverage/Regression/Retrieval metadata and ask how they should be used.

Pass observation:

- Coverage remains development-time operation→entrance audit, not runtime checklist;
- Regression remains artificial semantic regression evidence, not natural execution evidence;
- Retrieval remains structural sidecar, not semantic owner.

### FD-08 — Failure classification does not jump directly to semantic patch

State: a deployment output shows an error that current canonical semantics may already forbid.

Pass observation:

- first distinguishes packaging/source-loading/runtime-reachability/dispatch possibilities from genuine semantic defect;
- does not silently rewrite Trigger rows, runtime operations, field 4/6, or Regression expectations downstream.

## Result discipline

A single success does not establish general adequacy.

A single failure does not establish Trigger defect, protocol defect, or systematic weakness.

For any failure, preserve:

- actual input / actual user proposition / requested judgment;
- observable output failure;
- current canonical expectation;
- known facts versus inference;
- unresolved source-loading/reachability/dispatch/semantic-defect status.
