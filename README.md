# Jaeyoung Lee Portfolio

This repository builds the public researcher portfolio at
`https://sleepylee02.github.io/` with Hugo.

## Start here

- Workspace contract: [`WORKSPACE.md`](WORKSPACE.md)
- Agent guidance: [`AGENTS.md`](AGENTS.md)
- WOS workspace hub: [`00-workspace/README.md`](00-workspace/README.md)
- Current coordination: [`00-workspace/workstream/README.md`](00-workspace/workstream/README.md)
- Portfolio content model: [`docs/Explanation.md`](docs/Explanation.md)
- Hugo operations: [`docs/project_guide.md`](docs/project_guide.md)
- Content-update procedure: [`00-workspace/workstream/guides/content-update.md`](00-workspace/workstream/guides/content-update.md)

Current Attention and lifecycle state are owned by the Workstream index and its bound
record. This README remains a stable entry point and does not duplicate that state.

## Repository boundary

Public pages live under `content/`. Repository templates, static assets, configuration,
and the GitHub Pages workflow remain domain-native site artifacts. Verified publication
facts and the detailed content plan remain under `docs/`.

Raw source context under `docs/context/` is ignored and must never be copied into tracked
WOS records. A push to `main` can deploy through GitHub Actions, so local validation,
commit, push, and live-deployment verification remain separate gates.
