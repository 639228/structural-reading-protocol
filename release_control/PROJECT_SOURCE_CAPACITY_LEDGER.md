# Project Source Capacity Ledger

Status: `CURRENT_COUNT_CONFIRMED_17_OF_25 / V1.7_READINESS_SUCCESSOR_REPLACEMENT_AVAILABLE`

## Scope

This ledger records downstream Project-source capacity at the `1.0.1` documentation-patch materialization boundary. It does not alter canonical semantics, source roles, or repository/package history.

Project-source retirement means removal from the active Project-source inventory, not deletion of repository/package history.

## Current observed active Project-source inventory

Direct rediscovery before `1.0.1` materialization shows **17 / 25** active Project sources.

Soft ceiling: **20**.

Hard-limit reserve: **8 slots**.

### Foundational/current canonical/support/control owners (10)

1. `構造的読解プロトコル v8.3.18.txt`
2. `Trigger_Index_candidate_v0.1.txt`
3. `Coverage_Map_candidate_v0.8.txt`
4. `Materialization_Source_Manifest_v0.8.txt`
5. `Artifact_Retrieval_Index_candidate_v1.9.txt`
6. `Regression_Fixtures_candidate_v1.2.txt`
7. `Cross_Artifact_Consistency_Audit_v0.20.txt`
8. `Post_Materialization_Composition_Delta_Integration_Audit_v0.11.txt`
9. `Release_Engineering_Governance.md`
10. `Public_Distribution_Canonical_Snapshot_Handoff_v1.0.md`

### Current downstream/release support (7)

- `SOURCE_SHA256SUMS(1).txt`
- `TEST_PLAN(1).md`
- `FRESH_ENVIRONMENT_EXECUTION_RECORD_v1.0(1).md`
- `CURRENT_RELEASE_READINESS_STATE_v1.6(1).md`
- `LICENSE(1).md`
- `CITATION(1).md`
- `PUBLIC_LICENSE_AND_CITATION_AUTHORITY_v1.0(1).md`

## Readiness successor path

`CURRENT_RELEASE_READINESS_STATE_v1.7.md` may replace `CURRENT_RELEASE_READINESS_STATE_v1.6(1).md` one-for-one after direct Project-source admission verification.

Expected transition if only that successor is admitted and the predecessor is retired:
- temporary: `18 / 25`
- steady state after replacement: `17 / 25`
- steady-state reserve: `8`

Do not add package-internal verification artifacts to Project sources merely because they exist. Preserve capacity for future upstream handoffs or genuinely discriminative release evidence.
