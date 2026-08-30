# Portfolio WOS Workspace Hub

← [Portfolio repository](../README.md)

This directory is the target-local WOS control surface. It owns coordination artifacts,
not the portfolio's public content, fact registry, Hugo source, generated output, or
deployment state.

## Entry

- Contract: [`../WORKSPACE.md`](../WORKSPACE.md)
- Agent guidance: [`../AGENTS.md`](../AGENTS.md)
- Current coordination: [`workstream/README.md`](workstream/README.md)
- Managed Transit: [`.transit/README.md`](.transit/README.md)

The Workstream index owns Current Attention and points to lifecycle records. Domain
content remains at the final paths declared in `WORKSPACE.md`.

## Artifact map

- `workstream/records/` — multi-session effort identity and checkpoint
- [`workstream/maps/README.md`](workstream/maps/README.md) — optional Decision Maps
- `workstream/guides/` — reusable portfolio procedures
- [`workstream/log/README.md`](workstream/log/README.md) — material chronological changes
- [`.transit/README.md`](.transit/README.md) — ignored temporary context packages

One fact has one canonical owner. This hub must not reproduce publication facts,
content-plan detail, raw source context, or GitHub Pages runtime state.
