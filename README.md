# AI Office v2

A production-oriented workspace for a team of specialized AI agents. The repository describes roles, operating rules, skills, smoke checks and deployment scripts for an agent office that can coordinate product, backend, frontend, research, content, QA and design work.

This is the public-safe version. Live memory, personal context, server addresses, tokens and runtime sessions are not stored in this repository.

## What it demonstrates

- multi-agent role design and delegation model
- operator-first workflow for AI-assisted development
- reusable agent skills and references
- setup scripts for local or server-side agent workspaces
- health checks and consistency checks
- public templates for agent memory and team operations
- safety rules for secrets, public actions and gateway operations

## Agent roles

- `producer` - planning, ticket flow and coordination
- `orchestrator` - entry point and task routing
- `backend` - backend/API implementation
- `frontend` - UI implementation
- `tester` - QA, smoke checks and security review
- `design` - visual direction and interface polish
- `content` - copy, docs and publishing material
- `media` - media generation and processing
- `research` - domain research and synthesis
- `admin` - operations, finance and admin documentation

## Architecture

```text
User request
  -> producer/orchestrator
  -> specialist agent briefing
  -> isolated workspace
  -> review and quality gates
  -> report / handoff
```

Repository layers:

- `agents/` - public agent role templates
- `skills/` - reusable workflows and procedures
- `references/` - standards, checklists and operating docs
- `scripts/` - setup, validation and health utilities
- `configs/` - example configuration fragments
- `docs/` - public architecture and repository guide

## Quick start

```bash
git clone https://github.com/Glour/ai-office-v2.git
cd ai-office-v2
./scripts/setup.sh
./scripts/agent-health-check.sh
```

Some scripts are examples for a self-hosted agent environment. Real tokens, gateway configs and runtime state must be provided outside git.

## Public safety

This repository intentionally uses sanitized memory templates. Do not commit:

- real `TEAM_*.md` operational memory
- personal or customer context
- server IPs, SSH commands and gateway URLs
- `.env`, tokens, credentials or session files
- live agent session logs

See `SECURITY.md` and `docs/publication-checklist.md`.

## License

Proprietary. See `LICENSE`.
