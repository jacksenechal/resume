# Resume

A markdown-based resume with HTML and PDF publishing, plus an agentic workflow for maintaining tailored variants across roles and job applications.

## Quick Start

Edit `resume.md`, then run `./_publish` to generate `index.html` and `resume.pdf`.

Live version: [jacksenechal.com/resume](http://jacksenechal.com/resume/)

## Forking This Repo

This repo is designed to be forked and adapted. If you do:

1. Replace `resume.md` with your own content.
2. Replace [CONTEXT.md](CONTEXT.md) with your own factual context (role details, scale, constraints that agents should respect when tailoring your resume).
3. Keep [AGENTS.md](AGENTS.md) as-is — it contains the operational SOPs for the agentic workflow (branching, publishing, ATS formatting).

## Agentic Workflow

This repo uses AI coding agents (Claude Code, Copilot, Cursor, etc.) to tailor resumes for specific roles and job applications. The workflow is organized around branches:

- **`role/<target>`** — Reusable baselines for role archetypes (e.g., `role/engineering-lead`, `role/infrastructure-engineer`).
- **`job/<target>`** — One-off variants for specific job applications, branched from the closest role.
- **`main`** — The canonical resume and repo-level configuration.

Key files for agents:

| File | Purpose |
|------|---------|
| [AGENTS.md](AGENTS.md) | Operational SOPs: branching, workflow, publishing, ATS formatting |
| [CONTEXT.md](CONTEXT.md) | Personal factual context that agents must respect when tailoring content |
| `resume.md` | Source of truth for resume content |
| `_publish` | Generates `index.html` and `resume.pdf` from `resume.md` |

## Requirements

- pandoc or md2html
- google-chrome-stable or chromium

