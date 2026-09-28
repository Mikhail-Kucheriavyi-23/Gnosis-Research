# SELF-DIAGNOSTIC-0001 — Destination Verification Gate

Status: `UNVERIFIED`

This destination record is a migration contract. It is not a fabricated runtime result.

## Required runtime evidence

The destination may be marked verified only after a real Gnosis-Core runtime execution demonstrates:

1. `diagnostic_corpus/generate.py` executes successfully.
2. Exactly 4 `TransitionRecord` objects are produced and recovered.
3. Exactly 3 records are rejected and exactly 1 is accepted.
4. Every recovered record preserves `test-rule:diagnostic-policy`.
5. The SQLite persistence round-trip and durable graph verification succeed.
6. Diagnosis runs against recovered history.
7. `transitions.json`, `metadata.json`, and `diagnostic.json` are actually generated.
8. The resulting diagnostic artifact contains the required reflection fields.

## Migration rule

The Research destination is evidence-only. It does not become Core authority.

The original Core corpus remains in place until:

`destination runtime evidence` → `independent verification` → `Core CI boundary update` → `full Core CI pass` → `old dependency removal`.

No source deletion is authorized by this file.

## Provenance

- Source repository: `Mikhail-Kucheriavyi-23/Gnosis-Core`
- Source commit: `d42ec57166b706f954d7085dec11a938c31c1336`
- Generator blob SHA: `41eef2b7fba364732deff4fd128de340e38fbe81`
- Destination contract: `MIGRATION/SELF-DIAGNOSTIC-0001/REPRODUCTION-CONTRACT.json`
