# AGENTS.md

Guidance for working in this resume repo.

## Purpose

This repo is used to maintain Jack Senechal's resume and to produce tailored variants for:

- specific jobs
- broader role archetypes
- publishing to HTML and PDF

The source of truth is `resume.md`.
Generated artifacts are:

- `index.html`
- `resume.pdf`

Keep generated artifacts up to date in commits that change resume content.

## Branch Naming Conventions

Use scoped branch names.

### Job-specific resume variants

Use:

- `job/<target>`

Examples:

- `job/navan-ai-ex`
- `job/company-role-name`

These branches are for a concrete application to a specific posting/company.

### Reusable role-focused baselines

Use:

- `role/<target>`

Examples:

- `role/ai-tooling-engineer`
- `role/infrastructure-engineer`
- `role/engineering-manager`

These are reusable archetypes that future `job/...` branches can branch from.

## General Strategy

When tailoring a resume:

1. `git fetch --all --prune`
2. Review recent remote branches to see whether parallel work has landed that should be adopted.
3. Start from the most relevant existing branch rather than from `main` whenever possible.
4. Preserve ATS-friendly formatting.
5. Keep the narrative tight and role-specific.

### Typical branch selection strategy

- Start from the closest role-specific branch.
- Example: the Navan AI Developer Experience resume was branched from `origin/ai-tooling-engineer` and then customized.
- Do not accidentally push back onto the source branch if a new job-specific branch is intended.

## Workflow

Use this workflow for each meaningful iteration:

1. Edit files
2. Run `./_publish`
3. Commit changes
4. Open the PDF for inspection

In command form:

1. edit
2. `./_publish`
3. `git commit`
4. `open resume.pdf`

### Platform note

In this environment, `open` may not exist. Use the local equivalent if needed:

- `xdg-open resume.pdf`

The intent is always: inspect the generated PDF after each committed iteration.

## Publishing

The expected publishing command is:

- `./_publish`

`_publish` should regenerate:

- `index.html`
- `resume.pdf`

If tooling differs across environments, keep `_publish` working without breaking the normal workflow. Current implementation supports fallbacks when `pandoc` or `google-chrome-stable` are unavailable.

## ATS Formatting Guidance

Prefer simple, conventional section names and structures:

- `Summary`
- `Professional Experience`
- `Selected Projects`
- `Skills`
- `Education`

Guidelines:

- Use clear headings.
- Keep dates, company names, and titles easy to parse.
- Prefer standard formatting over decorative formatting.
- Keep skills concise and high-signal.
- Compress older experience when tailoring for a focused role.
- Preserve readability in both Markdown and generated PDF.

## Important Factual Context

Keep these facts straight when tailoring resume/cover letter content. Some prior drafts have unintentionally overstated or distorted them.

### Building Humane Technology / HumaneBench

- BHT is **not salaried employment**.
- It is a **volunteer / fractional-consulting-style** engagement.
- Time commitment has been **part-time, roughly ~20 hours/week**.
- It is **wrapping up**.
- Do not imply full-time staff employment unless explicitly directed.
- Do not overstate the work as if it matched the full scope of an internal AI developer platform org.
- The concrete production delivery was the **design, implementation, and publication of the benchmark**.
- There was also significant exploratory / strategic work around things like maturity models, possible real-time evals, and adjacent directions, but much of that remained investigative.
- Rough split of effort: approximately **2/3 consulting / leadership / strategy** and **1/3 technical**.

### Mirror Astrology

- Mirror is a **production-quality app**.
- It has **paying subscribers**, but only a small number.
- Approximate scale at the moment: **~5 monthly active subscribers** and **~5 daily active users**.
- It is fair to describe it as a real production app; do not imply significant scale.

## Recommendations / References Convention

Recommendations are currently kept out of the main body for ATS reasons and space discipline.

Current preference:

- if included, use a brief LinkedIn recommendations note in the footer rather than in the body
- avoid a large recommendations section in tailored job resumes unless specifically needed
- `References available upon request` is generally low value and should usually be omitted

Note: the LinkedIn recommendations line is primarily for human readers, not ATS benefit.

