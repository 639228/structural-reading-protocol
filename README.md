# 構造的読解プロトコル — Public Distribution

**Distribution:** `1.0.2`  
**Status:** **stable public release**

This package is a downstream public-distribution build of the canonical snapshot handed off as `PUBLIC_DISTRIBUTION_CANONICAL_SNAPSHOT_V1.0`.

It does not revise the upstream semantic specification.

## Quick Start

For a file-capable ChatGPT / LLM environment, the following is a distribution-side usage example. It is **not** a canonical system prompt and does not replace the Protocol or Trigger Index.

1. Download and extract this distribution.
2. Attach or otherwise make these two files directly available to the target model:
   - `runtime/構造的読解プロトコル v8.3.18.txt`
   - `runtime/Trigger_Index_candidate_v0.1.txt`
3. Send a bootstrap instruction such as:

```text
添付した2ファイルをruntime packageとして使用してください。構造的読解プロトコル本文をnormative/semantic owner、Trigger Indexをruntime dispatchとして扱ってください。Trigger IndexはProtocol本文を置き換えず、固定checklistとして扱わないでください。以後の質問にはこのruntime packageを使用して回答してください。
```

4. After the model has loaded the two roles correctly, ask the question you actually want answered.

For ordinary use, `developer_research/` and `evidence_provenance/` do not need to be loaded. See `INSTALLATION.md` for the distribution-side loading contract.

## Runtime: what you actually need

For ordinary runtime use, use these two files together:

1. `runtime/構造的読解プロトコル v8.3.18.txt`
   - normative specification
   - semantic operation owner
   - Reference Gate basis

2. `runtime/Trigger_Index_candidate_v0.1.txt`
   - observable runtime sign → existing operation dispatch
   - runtime entrance / necessity / routing / stop semantics

The protocol body and Trigger Index have different roles. The Trigger Index does not replace the protocol body.

Do not turn the Trigger Index into a fixed checklist. A visible sign is not by itself a requirement to start every related operation. `NO START`, `NO FIRE`, and `STOP` are valid runtime results when the canonical conditions say so.

## Minimal use

1. Make both files in `runtime/` directly available to the target model or execution environment.
2. Preserve the protocol body as the normative semantic owner and the Trigger Index as the runtime dispatch layer.
3. Prefer direct access to these canonical files over rewriting them into a new summarized rule set.
4. Keep developer/research and evidence/provenance artifacts outside the ordinary runtime path unless they are needed for verification, research, or provenance work.

See `INSTALLATION.md` for the distribution-side loading requirements.

## Package layers

### `runtime/`
Minimal runtime package.

### `developer_research/`
Development and verification support:

- Coverage Map — development-time operation → entrance coverage audit; not a runtime checklist.
- Regression Fixtures — artificial semantic regression baseline; not natural execution evidence.
- Artifact Retrieval Index — structural retrieval sidecar; not a semantic owner.
- Materialization Source Manifest — projection/provenance support; not runtime semantics.
- Cross Artifact Consistency Audit — bounded projection/retrieval consistency audit.

### `evidence_provenance/`
Current supplied provenance carrier for composition-delta integration.

The current input set does **not** contain every natural execution replay or historical evidence carrier referenced by the support artifacts. Missing carriers are not reconstructed from conversational memory or embedded references.

### `historical_archive/`
No historical archive payload is included in this stable public distribution. Checkpoint/predecessor history remains outside ordinary runtime use.

### `release_control/`
Downstream source-selection, intake, release-engineering records, and package checks.

## Evidence boundary

Current support artifacts contain bounded artificial regression and bounded projection/provenance results. This distribution does **not** claim:

- protocol-wide adequacy,
- natural whole-protocol end-to-end execution,
- reproducibility across all models or environments,
- absence of systematic weakness,
- historical firstness or absence of prior art,
- universal performance improvement.

The current handoff also does not authorize a Trigger semantic repair, a new runtime operation, new Trigger rows, or field 4 / field 6 semantic changes.


## License and citation

- Creator / Licensor: `639228`
- License: Creative Commons Attribution 4.0 International (`CC BY 4.0`)
- DOI: not yet assigned
- Repository: https://github.com/639228/structural-reading-protocol

See `LICENSE.md` for licensing scope and attribution terms, and `CITATION.md` for the preferred citation form.
The authoritative downstream metadata decision is preserved in `release_control/PUBLIC_LICENSE_AND_CITATION_AUTHORITY_v1.0.md`.

## Version identities

These versions are independent:

- Protocol: `v8.3.18`
- Trigger Index: `v0.1`
- Coverage: `v0.8`
- Manifest: `v0.8`
- Retrieval: `v1.9`
- Regression: `v1.2`
- Cross audit: `v0.20`
- Integration audit: `v0.11`
- Distribution: `1.0.2`

A downstream Distribution version change does not imply an upstream semantic revision.

## Release status

The prepared fresh-environment observation set FD-01..FD-08 passed 8 / 8 in one operator-reported fresh Project execution at the bounded strength recorded in `tests/fresh_environment/EXECUTION_RECORD.md`. That result is not generalized to protocol-wide adequacy, natural whole-protocol execution, or cross-model/cross-environment reproducibility.

`tests/fresh_environment/TEST_PLAN.md` is preserved as the original pre-run specification; its historical status line is not the current execution-state owner. Use `EXECUTION_RECORD.md` for the executed result.

The authoritative Creator / Licensor identity and CC BY 4.0 license are integrated into this distribution. The prior LICENSE / CITATION metadata blockers remain closed after stable-release materialization verification.

Distribution `1.0.2` is a documentation-only stable patch over `1.0.1`. It adds a non-canonical Quick Start usage example and records the assigned public repository URL. It does not revise runtime semantics, evidence strength, or canonical source identity. The prior stable releases remain part of release history.

For the consolidated current release-engineering judgment, see `release_control/CURRENT_RELEASE_READINESS_STATE.md`.

## 謝辞

本Protocolには、信州大学で学んでいた際に佐々木寛氏から伝達された「小説におけるリズムとは、予測可能な未来である」という定義、および篠原成彦氏から伝達された「新しいこと／他の知の体系と繋がっていること／100％理屈であること／明晰であること」の四条件が、明示的な知的由来として含まれている。

両氏に感謝する。

なお、これらを基礎として本Protocolで行われた後続の操作的展開まで、両氏自身が同じ形で体系化・承認したものとして扱うものではない。

また、本Protocolにおける私の理解や操作的展開が、両氏の本来の意図を完全に再現していると主張するものでもない。情報の受容には、当然ながら歪み、変形、誤読の可能性がある。

だが、それらを踏まえてなお、この成果物が、両氏から受け取った教えを一つの起点として形成されたものであることに変わりはない。

これらの教えを受け取る機会を得たことに、深く感謝する。

