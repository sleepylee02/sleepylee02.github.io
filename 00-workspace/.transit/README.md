# Managed Transit

This ignored directory is available only for temporary context packages crossing a real
context boundary.

- The tracked [Handoff Outbox](handoffs/README.md) preserves the runtime path; actual
  bundles live under ignored `handoffs/<handoff-id>/` paths.
- It is never canonical portfolio, content, fact, Workstream, or deployment state.
- Preparing a packet does not deliver it.
- Never copy ignored `docs/context/` material or private publication inputs here without
  an exact public-safety and redaction review.
- Do not use Transit to publish site assets or generated Hugo output.
- Cleanup remains user-controlled; no automatic cleanup runs.
