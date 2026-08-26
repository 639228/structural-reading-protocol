# Project Source Capacity Ledger

Status: `CURRENT_COUNT_CONFIRMED_17_OF_25 / V1.8_READINESS_SUCCESSOR_AVAILABLE`

## Scope

This ledger records downstream Project-source capacity at the `1.0.2` documentation-patch materialization boundary. It does not alter canonical semantics, source roles, or repository/package history.

Project-source retirement means removal from the active Project-source inventory, not deletion of repository/package history.

## Current observed active Project-source inventory

Direct rediscovery before `1.0.2` materialization shows **17 / 25** active Project sources.

Soft ceiling: **20**.

Hard-limit reserve: **8 slots**.

Current release-state owner at materialization start:
- `CURRENT_RELEASE_READINESS_STATE_v1.7(1).md`

## Readiness successor path

`CURRENT_RELEASE_READINESS_STATE_v1.8.md` may replace `CURRENT_RELEASE_READINESS_STATE_v1.7(1).md` one-for-one after direct Project-source admission verification.

Expected transition if only that successor is admitted and the predecessor is retired:
- temporary: `18 / 25`
- steady state after replacement: `17 / 25`
- steady-state reserve: `8`

Do not add package-internal Work Unit 08 or checksum files to active Project sources merely because they exist. Preserve capacity for future upstream handoffs or genuinely discriminative release evidence.
