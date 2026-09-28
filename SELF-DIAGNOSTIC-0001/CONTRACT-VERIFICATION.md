# SELF-DIAGNOSTIC-0001 Contract Verification

This verifier checks the migration contract only. It does not execute Gnosis-Core and does not claim runtime evidence.

Required invariants:
- artifact_id is SELF-DIAGNOSTIC-0001
- source repository is Mikhail-Kucheriavyi-23/Gnosis-Core
- baseline commit is d42ec57166b706f954d7085dec11a938c31c1336
- expected transitions are 4 total, 3 rejected, 1 accepted
- recovery and diagnosis are required
- recovered rule is test-rule:diagnostic-policy
- the Research artifact is not Core state or execution authority
- runtime evidence flags remain false
- source deletion remains prohibited

Result: contract-valid / runtime-unverified.
