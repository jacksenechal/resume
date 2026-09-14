# AGENTS.md

Guidance for working in this resume repo.

## Purpose

This repo maintains **only two kinds of thing**:

- `main` — Jack Senechal's **canonical résumé** (`resume.md`), the public source of truth,
  published to HTML and PDF.
- `role/*` branches — reusable **role archetypes** (generic role positionings, e.g.
  `role/technology-executive`, `role/engineering-manager`, `role/infrastructure-engineer`,
  `role/engineering-lead`, `role/ai-tooling-engineer`). Archetypes are **generic**: no company
  names, no per-application tailoring.

Generated artifacts (`index.html`, `resume.pdf`) are kept up to date in commits that change
résumé content.

## This repo is PUBLIC — per-job tailoring does NOT happen here

**Never create `job/*` branches in this repo.** A branch named `job/<company>` publicly advertises
that Jack applied there; the whole point of the current setup is that the application list stays
private. `job/*` branches have been retired and deleted.

Per-job résumé tailoring lives in the **private jobs repo**:

- Copy the closest archetype into the application folder:
  `git -C ~/workspace/resume show role/<name>:resume.md > ~/workspace/jobs/applications/<id>/resume.md`
- Tailor it there, then render with `~/workspace/agent-tools/skills/job-search/scripts/make_resume_pdf.sh`
  (self-contained; does not need this repo at runtime), to `applications/<id>/Resume - <Name> - <Role>.pdf`
  (always the named file, never a bare `resume.pdf`).
- Full workflow: the `job-search` skill's `SKILL.md` (Stage 2) and `~/workspace/jobs/CLAUDE.md`
  ("Resume Workflow").

So from a tailoring session this repo is effectively **read-only** (read `main` or a `role/*`
archetype via `git show`, never check out or branch).

## When to edit in THIS repo

Only to change the canonical résumé or an archetype itself:

- **`main`**: update Jack's canonical résumé (facts, structure, house style).
- **`role/*`**: refine a generic archetype so future applications branch from a stronger base.
  Keep archetypes generic — never add a company name or posting-specific content.

### Keeping archetypes current with main

Archetypes drift behind `main` as the canonical résumé gains fixed facts and convention
changes; a stale archetype tailors from wrong facts. They are kept current **lazily** — each is
refreshed the next time its role is tailored (job-search skill, Stage 2 step 1b) — plus an
on-demand pass:

- `~/workspace/agent-tools/skills/job-search/scripts/sync_archetypes.sh` (`/job-search
  sync-archetypes`) merges `main` into each `role/*`, regenerates artifacts, and pushes the ones
  that merge cleanly. Generated-file conflicts (`index.html`, `resume.pdf`) are noise and get
  regenerated; a `resume.md` conflict means the archetype has diverged too far for a merge.
- A conflicted archetype needs a **content refresh**, not a forced merge: re-derive its
  `resume.md` from current `main` plus the role's positioning (strip company/sector specifics,
  apply the conventions below and current `facts.md`), `./_publish`, commit, push. This resets a
  clean, recent merge-base so future syncs stay thin.

Never `rebase` a public `role/*` branch (it force-pushes shared history); always merge or refresh.

### Workflow for a main/archetype edit

1. Check out `main` or the `role/*` archetype.
2. Edit `resume.md`.
3. Run `./_publish` (regenerates `index.html` and `resume.pdf`).
4. Inspect the PDF (`xdg-open resume.pdf`; `open` may not exist in this environment).
5. Commit the source and the generated artifacts together; push.

`_publish` uses pandoc → HTML → headless Chrome → PDF. Keep it working across environments
(it has fallbacks when `pandoc` or `google-chrome-stable` are unavailable). The per-job render
script (`make_resume_pdf.sh`) embeds the same styling from `_pandoc/header_styles.html`, so if you
change the résumé CSS here, update that script too (or note the drift).

## Writing conventions (canonical set lives in the jobs repo)

The résumé voice/style conventions are maintained in `~/workspace/jobs/CLAUDE.md` ("Resume
Workflow") and `~/workspace/jobs/strategy/` (`facts.md`, `voice-profile.md`). Apply them here too:

- **Bolding = structural anchors only** (bullet-leading labels, section/category labels, project
  names). No inline emphasis on metrics, tech, or awards; no bold inside recommendation quotes.
  (Tailored per-job variants may add role-specific emphasis; the canonical/archetype base stays clean.)
- **Summary is a positioning statement**: frame overcoming as positive results; never lead with
  others' failures ("mass departures", "single engineer") — that context belongs in the body.
- **Tense**: gerund for current-role ongoing responsibilities ("Serving as fractional CTO"), past
  tense for finished work and past roles.
- **Register**: subject-elided / zero-subject (verb-led, pronoun suppressed); no relative clauses
  grafted onto noun phrases.
- **No em/en dashes** except the `*— Name, Title*` recommendation attributions. Never alter words
  inside recommendation quotes.
- **Facts**: `~/workspace/jobs/strategy/facts.md` is the source for verifiable particulars.

## ATS Formatting Guidance

Prefer simple, conventional section names and structures (the canonical résumé currently uses
`Summary`, `Professional Experience`, `Leadership Practice`, `Selected Open Source`, `Education`,
`Recommendations`; archetypes may vary the middle sections):

- Clear headings; dates, company names, and titles easy to parse.
- Standard over decorative formatting; concise, high-signal skills/practice.
- Compress older experience when an archetype is focused.
- Preserve readability in both Markdown and the generated PDF.

## Interview Prep Guides

**Never in this repo.** Interview prep documents contain named interviewers, hiring managers and
recruiters, interview locations, and comp negotiation strategy. This repo is public.

They belong in the private job-search repo at
`~/workspace/jobs/applications/<id>/interview-prep-<company>.md`. The guide for writing one is
`~/workspace/jobs/strategy/interview-prep-guide.md`.

The same rule covers anything with third-party names, comp figures, or private strategy: if it is
not the résumé itself, it does not go here.

## Personal Context

Personal context (project narratives, factual guardrails, self-assessment) is maintained outside
this repo, in the private jobs repo. The calling agent is responsible for providing relevant
context when requesting résumé edits.
