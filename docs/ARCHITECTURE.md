# Architecture Overview

This document describes the **public-safe architecture** of ZANDELA / LIVING SYSTEM.

## Governing flow

```text
Canonical Git state
    ↓
Deterministic validation
    ↓
Human promotion / ratification
    ↓
Runtime projection
    ↓
Public renderer
```

The central architectural rule is that runtime infrastructure may serve, index, render, and distribute approved state, but it does not become an independent source of institutional truth.

## Layers

### 1. Canonical layer
Owns ratified project state, evidence references, ontology, gate history, authority records, schemas, and build evidence.

### 2. Validation and promotion layer
Enforces schemas, invariants, publication boundaries, gate acceptance criteria, and adversarial checks before state is promoted.

### 3. Projection layer
Produces public-safe and runtime-friendly views of canonical state. Projection records retain lineage to their source version and commit.

### 4. Rendering layer
Presents approved state through the public website and related surfaces.

### 5. Intelligence layer
Later AI-assisted retrieval, interpretation, and interface composition sit above canonical truth and do not silently rewrite it.

## Authority model

The system separates:
- proposal;
- validation;
- ratification;
- canonical state;
- publication.

Agents may execute bounded work. Human authority remains explicit at material state transitions.

## Execution model

Authorized work follows:

```text
authorized gate
→ controller decomposition
→ bounded worker packages
→ deterministic validation
→ integrated candidate
→ independent review
→ human ratification
→ canonical promotion
```

Non-material defects are handled through a bounded remediation loop:

```text
hypothesis → test → smallest bounded fix → revalidate → continue
```

The loop stops when a material authority boundary is reached.

## Public boundary

This overview intentionally omits internal prompts, sensitive evidence, private implementation details, credentials, and unpublished canonical records.
