# Public Build Notes

ZANDELA separates engineering evidence from publication narrative.

## Engineering evidence stack

### Commit
Durable engineering evidence. Material commits use a human-readable subject plus machine-readable trailers.

### Checkpoint
The institutional promotion record for a material state transition. Checkpoints are maintained in both human-readable and machine-readable form.

### Build note
A concise explanation of:
- what changed;
- why it mattered;
- what was tested;
- what authority boundary was preserved;
- what remained unresolved.

### Public post
A sanitized lesson derived from the build note.

## Why this matters

A public technical narrative should be understandable without overstating maturity or exposing private mechanics.

The public layer therefore preserves:
- provenance;
- evidence boundaries;
- maturity boundaries;
- authority boundaries;
- failure/correction history where publication-safe.

It intentionally excludes:
- secrets;
- credentials;
- customer/private evidence;
- internal prompts;
- raw agent traces;
- unpublished architecture;
- sensitive operational detail.

## Example

A useful public lesson is not:

> "AI built the whole system automatically."

A better representation is:

> "Bounded agents were allowed to execute implementation work, while deterministic validators and human ratification controlled whether candidate state could become canonical."

That distinction is central to ZANDELA.
