# Installation / Runtime Loading

[日本語](INSTALLATION.md)

This document describes distribution-side loading only. It does not replace or summarize the canonical runtime semantics.

## Recommended first-time ChatGPT setup

Create a new ChatGPT Project and add these four files:

1. `README.md`
2. `INSTALLATION.md`
3. `runtime/構造的読解プロトコル v8.3.18.txt`
4. `runtime/Trigger_Index_candidate_v0.1.txt`

`README.md` and `INSTALLATION.md` are distribution/loading guides. The canonical runtime pair is:

- `runtime/構造的読解プロトコル v8.3.18.txt`
- `runtime/Trigger_Index_candidate_v0.1.txt`

If you already understand the loading method, those two files are the minimum runtime set.

## ChatGPT procedure

1. Create a new Project.
2. Project instructions may be left blank for this baseline setup.
3. For first-time use, add README, INSTALLATION, the Protocol body, and the Trigger Index to the Project.
4. Start a new chat inside the Project.
5. Send the bootstrap shown in the Japanese `README.md` once at the start of that chat.
6. Then paste or attach the material to analyze and ask the actual question.
7. When starting a separate new chat while Project instructions remain blank, send the bootstrap again at the start of that chat.

This is distribution-side loading guidance, not a canonical system prompt.

## Loading contract

1. Treat the Protocol body as the normative specification and semantic operation owner.
2. Treat the Trigger Index as the observable-sign → existing-operation runtime dispatch layer.
3. Keep the two artifacts distinct. Do not merge them into a rewritten substitute specification.
4. Do not treat the Trigger Index as a fixed checklist.
5. A visible sign alone does not force an operation to start; preserve valid `NO START`, `NO FIRE`, and `STOP` results.
6. Do not substitute Coverage, Regression, Retrieval, Manifest, audit, or historical materials for the runtime pair.
7. When direct file access is available, prefer the canonical runtime files over reconstructing their rules from memory or a secondary summary.
8. If exact-file verification is required, compare the runtime file hashes with `release_control/SOURCE_SHA256SUMS.txt`.

## Optional verification/research inputs

The files in `developer_research/`, `evidence_provenance/`, `release_control/`, and `tests/` are not required for ordinary reading. Use them only when the current work actually requires regression inspection, coverage auditing, provenance tracing, or release/deployment validation.

## Language boundary

The canonical runtime is Japanese. The English distribution documents are navigation/loading guides, not translated canonical runtime artifacts. Equivalent English-language or translated-runtime behavior has not been established by current evidence.
