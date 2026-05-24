# Repository structure and memory model

This public repository contains templates for an AI-agent office. It does not contain live memory or private operator context.

## Layers

- `agents/` - role-specific agent templates
- `skills/` - reusable procedures
- `references/` - standards and checklists
- `scripts/` - setup and validation utilities
- `configs/` - example configuration fragments
- `docs/` - public documentation

## Memory files

`TEAM_*.md` and `agents/*/MEMORY.md` in this repository are examples. In production, live memory is deployment data and must stay outside public git.

## Rule

Public repo = templates and architecture. Server = secrets, sessions, personal context and production state.
