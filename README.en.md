# Structural Reading Protocol — Public Distribution

[日本語](README.md)

**Distribution:** `1.0.4`  
**Status:** **stable public release**

### Not a prompt for making ChatGPT “think harder,” but an execution architecture for controlling
### **what needs to be examined, why it needs to be examined, and when to stop.**

> **It does not add capabilities; it designs the route by which existing capabilities are reached and used.**

ChatGPT can summarize, analyze, compare, form hypotheses, research, and evaluate. In long or complex work, however, a different problem can appear: because many operations are possible, it may be unclear which ones should actually be used now.

Examples include weakening a supported judgment merely because another possibility can be imagined; drifting from the user's question to an easier or stronger one; treating “rare” as if it meant “historically first”; starting source research when the current judgment does not depend on it; or continuing exploration after the requested judgment is already established.

The Structural Reading Protocol treats these as execution-control problems. It integrates close reading, active inquiry, research, evaluation, state management, and audit while preserving the principle that only operations needed for the current judgment should start.

## What is different from ordinary prompting?

Instructions such as “read carefully,” “think deeply,” or “research if necessary” mainly ask for capabilities. This protocol also specifies runtime conditions:

- what observable sign makes an operation a candidate;
- whether that operation is actually necessary now;
- what difference it is supposed to discriminate;
- whether the current judgment already stands without that inspection;
- where execution should route if another operation is needed;
- when the operation should stop.

The attached **Trigger Index** is the runtime dispatch layer for these decisions. Its six fields are: observable firing sign, candidate operation, discrimination target, condition under which the current judgment stands without inspection, destination if needed, and stop condition.

A candidate operation is not an automatic start. `NO START`, `NO FIRE`, and `STOP` are valid runtime results under their canonical conditions.

## It is not an “analyze everything deeply” prompt

The Protocol does not maximize analysis volume. It normally reads at the minimum resolution sufficient for the current judgment and increases resolution only where local wording, syntax, reference, voice, time, or other structure can materially change that judgment.

Its target is **necessary and sufficient analysis, not maximum analysis**.

## Typical uses

This architecture is intended for tasks such as:

- close reading of fiction, criticism, and difficult prose without collapsing local and global structure;
- keeping multiple meaning paths, unresolved alternatives, and actual contradictions distinct;
- testing hypotheses without letting merely imaginable possibilities weaken established claims;
- moving to originals, sources, transmission paths, research history, or prior work only when the current judgment depends on those differences;
- distinguishing “more could be considered” from “more must be considered” and stopping when further work adds no material discrimination;
- using reading, inquiry, research, comparison, and evaluation without flattening them into one undifferentiated procedure.

## Language status

The canonical runtime artifacts in this release are written in Japanese.

This English README and `INSTALLATION.en.md` are distribution/navigation documents. They are **not** English translations of the Protocol or Trigger Index and do not constitute an English canonical runtime.

Equivalent semantic behavior with English-language user input or translated runtime artifacts has not been established by the current evidence.

# Using it in ChatGPT

## Recommended first-time setup

For a first trial in ChatGPT, create a new Project and add these **four files** to the Project's sources / reference materials:

1. `README.md`
2. `INSTALLATION.md`
3. `runtime/構造的読解プロトコル v8.3.18.txt`
4. `runtime/Trigger_Index_candidate_v0.1.txt`

The first two are distribution and installation guides. The canonical runtime pair is the Protocol body plus the Trigger Index.

### Minimum runtime setup

Once you understand the loading method, the minimum runtime set is only:

1. `runtime/構造的読解プロトコル v8.3.18.txt`
2. `runtime/Trigger_Index_candidate_v0.1.txt`

## ChatGPT setup outline

1. Create a new ChatGPT Project.
2. Project instructions may be left blank for this baseline setup.
3. For a first-time setup, add the four files listed above to the Project.
4. Start a new chat inside that Project.
5. Send the Japanese bootstrap shown in `README.md` once at the start of the chat.
6. Then paste or attach the material to analyze and ask the actual question in ordinary language.
7. If you start a separate new chat while Project instructions remain blank, send the bootstrap again at the start of that chat.

The bootstrap is distribution-side loading guidance, not a canonical system prompt. Do not replace the canonical runtime files with a summary or translation.

For the full Japanese step-by-step guide, see `README.md` and `INSTALLATION.md`.

## Package layers

- `runtime/` — minimum runtime package
- `developer_research/` — Coverage, Regression, Retrieval, Manifest, and verification support
- `evidence_provenance/` — supplied provenance / integration evidence
- `historical_archive/` — historical layer / navigation
- `release_control/` — source selection, intake, checksums, and release-engineering records
- `tests/` — fresh-environment test plan and saved execution record

Coverage is not a runtime checklist. Regression is artificial semantic regression evidence rather than natural runtime evidence. Retrieval is a structural sidecar rather than a semantic owner.

## Evidence boundary

This distribution does **not** claim to have established:

- protocol-wide adequacy;
- natural whole-protocol execution;
- reproducibility across all models or environments;
- absence of systematic weakness;
- historical firstness or absence of prior art;
- universal performance improvement;
- equivalence of English-language input or translated runtime artifacts with the Japanese canonical runtime.

The saved fresh-environment observation records `8 / 8` prepared FD cases passing in one fresh Project execution. That result is not generalized beyond its recorded strength.

## License and citation

**Creator / Licensor:** `639228`  
**License:** Creative Commons Attribution 4.0 International (`CC BY 4.0`)  
**DOI:** not assigned  
**Repository:** https://github.com/639228/structural-reading-protocol

`See `LICENSE.md`for the standard license text,`NOTICE.md`for scope and attribution guidance, and`CITATION.md` for preferred citation information.`

## Versions

- Protocol: `v8.3.18`
- Trigger Index: `v0.1`
- Coverage: `v0.8`
- Manifest: `v0.8`
- Retrieval: `v1.9`
- Regression: `v1.2`
- Cross audit: `v0.20`
- Integration audit: `v0.11`
- Distribution: `1.0.4`

Protocol version and Distribution version are separate. Documentation-only changes do not revise the Protocol version.
