# Governed Architecture — ZANDELA / LIVING SYSTEM

This document is derived from the ratified Gate 5 technical architecture in the private canonical repository.

## Governing architecture

```text
Git canonical state
→ deterministic validation
→ human promotion
→ runtime projection
→ public renderer
```

The architectural rule is that **Git remains canonical**. Runtime infrastructure such as Postgres/Supabase may serve as a projection/query layer, but it does not acquire authority to redefine institutional state.

## Runtime projection boundary

A projection record is expected to retain lineage to canonical state, including:

- canonical source ID;
- canonical record version;
- source commit SHA;
- projection version;
- projected timestamp;
- projection hash.

Runtime projection must not silently strengthen:

- maturity;
- authority;
- publication state;
- evidence strength;
- ratification state.

## Deployment and security doctrine

The ratified architecture requires:

- production deployments to originate from promoted commits;
- previews to remain non-canonical;
- deployment identity to remain bound to source commit identity;
- secrets to remain outside canonical repository content;
- public rendering to use public-safe projection only;
- runtime/operational systems to have no canonical Git write authority;
- R1 to have no AI dependency.

## Fail-closed behavior

The architecture is designed to fail closed when required provenance, ratification, disclosure state, schema validity, or projection integrity is missing.

## Public limitation

This is a sanitized architectural summary. It is not a production-security certification and does not expose private implementation details or credentials.
