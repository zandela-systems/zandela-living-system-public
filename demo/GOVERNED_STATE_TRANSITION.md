# Demo Walkthrough — Governed State Transition

This walkthrough shows the behavior ZANDELA is designed to preserve.

## Scenario

A system proposes a public maturity change for a project.

### Step 1 — Candidate
The proposed change enters candidate state. It is **not canonical** and must not appear publicly merely because an AI or worker produced it.

### Step 2 — Validation
Deterministic validators check the proposal against schemas, evidence references, maturity rules, publication constraints, and prior ratified state.

### Step 3 — Review
Adversarial and/or independent review checks whether the candidate can bypass authority, disclosure, or evidence constraints.

### Step 4 — Human authority
If the transition is consequential, a human ratification event is required.

### Step 5 — Canonical promotion
Only after the required checks and authority event does the new state become canonical.

### Step 6 — Public-safe projection
The renderer receives an approved projection of canonical state. Runtime infrastructure may render it but cannot strengthen it.

## Expected failure behavior

If evidence, authority, disclosure, or lineage is missing, the transition should fail closed and canonical state should remain unchanged.

This is the governing behavior behind the public Living System, not a claim that every later runtime surface is already implemented.
