# SELF-DIAGNOSTIC-0001 — Provenance Manifest

Status: MIGRATION PREPARATION — source remains in Gnosis-Core.

## Source
- Repository: `Mikhail-Kucheriavyi-23/Gnosis-Core`
- Source path: `diagnostic_corpus/SELF-DIAGNOSTIC-0001/`
- Generator: `diagnostic_corpus/generate.py`
- Source baseline commit: `d42ec57166b706f954d7085dec11a938c31c1336`

## Meaning
This artifact is reproducible diagnostic evidence produced by a controlled runtime scenario with durable SQLite persistence and recovery.

## Verification contract
- 4 transition records are expected.
- 3 records are rejected.
- 1 record is accepted.
- recovered records preserve `test-rule:diagnostic-policy`.
- durable graph verification must succeed.

## Migration rule
This manifest does not authorize deletion or movement of the source. The source remains authoritative for provenance until the destination artifact is independently verified and the Core CI references are updated.

## Trust boundary
The artifact is evidence, not canonical Core state and not execution authority.