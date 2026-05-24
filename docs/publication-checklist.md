# Public publication checklist

Use this checklist before pushing a branch intended for a public portfolio repository.

## Current tree

- `git status --short` is clean
- no `.env`, tokens, browser sessions, databases or logs are tracked
- agent memory files contain templates only
- hostnames, public IPs and private paths are replaced with placeholders
- README explains the project without private operational context

## Git history

If real secrets or private context ever existed in history, do not make the repository public until history is purged or a clean public repository is created.

## Runtime data

Keep live runtime under server-local state directories or secret managers. Public git contains only templates.
