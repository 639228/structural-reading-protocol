# Installation / Runtime Loading

This document describes distribution-side loading only. It does not replace or summarize the canonical runtime semantics.

## Required runtime inputs

The minimum runtime set is:

- `runtime/構造的読解プロトコル v8.3.18.txt`
- `runtime/Trigger_Index_candidate_v0.1.txt`

Both must be available to the target execution environment.

## Loading contract

1. Load or attach the protocol body as the normative specification and semantic operation owner.
2. Load or attach the Trigger Index as the observable-sign → operation dispatch layer.
3. Keep the two artifacts distinct. Do not merge them into a rewritten substitute specification.
4. Do not substitute Coverage, Regression, Retrieval, Manifest, audit, or historical materials for the runtime pair.
5. When the environment permits direct file access, prefer direct access to the canonical runtime files over reconstructing their rules from memory or a secondary summary.
6. If exact-file verification is required, compare the runtime file hashes with `release_control/SOURCE_SHA256SUMS.txt`.

## Environment-specific bootstrap

No platform-specific installer or system-prompt wrapper is canonicalized in the supplied snapshot. A future distribution-specific bootstrap may be added downstream, but it must preserve the canonical semantic ownership and must not add, remove, strengthen, or weaken runtime rules.

Until such a bootstrap is validated, the portable installation path is direct loading of the two runtime artifacts above.

## Optional verification/research inputs

The files in `developer_research/` and `evidence_provenance/` are optional for ordinary runtime use. Load them only when the current work requires regression inspection, coverage auditing, retrieval/provenance tracing, or release/deployment validation.
