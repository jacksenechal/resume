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

## Interview Prep Guides

When preparing for a specific job opportunity, generate an interview prep document alongside any resume tailoring. Save it as `interview-prep-<company>.md` in the repo root.

### Research phase

Gather information in parallel before writing anything:

1. **Company research** — Fetch the company website, about page, careers page. Web search for recent news, funding, growth metrics, and leadership profiles. Understand what they build, their stage, their tech stack, and their culture.
2. **Role research** — Analyze the job listing for explicit and implicit requirements. Identify which product domains or teams this role maps to.
3. **People research** — Look up the interviewer(s) and key hiring-chain people (recruiter, hiring manager, CTO, etc.) on LinkedIn. Note backgrounds, tenure, communication style, and any commonalities with the candidate.
4. **Resume context** — Read the current resume to map strengths and gaps against the role requirements.

### Document structure

Use this outline:

1. **Quick Company Brief** — What they do, founding story, growth metrics (ARR, GMV, headcount), funding stage, tech stack, location/remote policy. Include a "What They Actually Build" subsection breaking down their product areas.
2. **Key People** — Profiles of the interviewer, hiring manager, CTO, CEO, and other relevant leaders. Include career backgrounds and key insights about what they'll care about.
3. **Your Interview: What to Expect** — Interview format (recruiter screen, technical, etc.), what the interviewer is evaluating, and the dynamic (did they reach out to you, or did you apply?).
4. **What to Lean Into** — Map the candidate's strongest experiences to the role's requirements. Group by theme (e.g., "Crown Jewel Experience," "Startup DNA," "Stack Alignment," "Domain-Adjacent Experience," "Leadership Style"). Be specific — cite particular projects, metrics, and teams.
5. **Growth Areas** — Honest assessment of gaps. For each, provide:
   - A concise framing of what to say if pressed
   - What NOT to oversell (especially if the interviewer has deep expertise in that area)
6. **Questions to Ask** — Grouped by category (role/team, product/technical, culture/process). These should demonstrate research and genuine curiosity. End with a "close strong" question about next steps.
7. **Key Talking Points** — 4-5 punchy one-liners to weave into conversation naturally.
8. **Salary/Comp Notes** — Stage-appropriate ranges, deflection strategies, and context for negotiation.
9. **Red Flags to Watch For** — Things the candidate should evaluate about the company during the interview. Be candid.
10. **One-Liner** — A closing pitch sentence that ties the candidate's experience to the company's mission.

### Principles

- **Be honest about gaps.** Never coach the candidate to claim expertise they don't have — especially when the interviewer has deep domain knowledge.
- **Do the research.** The value is in specific, verified details — not generic interview advice. Company metrics, interviewer backgrounds, and product specifics make the guide actionable.
- **Match the interview stage.** A recruiter screen needs different prep than a technical deep-dive or a founder chat. Tailor the emphasis accordingly.
- **Serve the candidate's evaluation too.** The interview is bidirectional. Red flags and questions to ask are as important as talking points.

## Personal Context

Personal context (project narratives, factual guardrails, self-assessment) is maintained outside this repo. The calling agent is responsible for providing relevant context when requesting resume edits.
