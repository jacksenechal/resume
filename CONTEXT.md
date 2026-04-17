# Personal Context

Factual context for tailoring resume and cover letter content. Agents should read this file before making content changes to `resume.md`.

**If you forked this repo:** replace this file with your own details.

## Building Humane Technology / HumaneBench

Keep these facts straight — some prior drafts have unintentionally overstated or distorted them.

- BHT is **not salaried employment**.
- It is a **volunteer / fractional-consulting-style** engagement.
- Time commitment has been **part-time, roughly ~20 hours/week**.
- It is **wrapping up**.
- Do not imply full-time staff employment unless explicitly directed.
- Do not overstate the work as if it matched the full scope of an internal AI developer platform org.
- The concrete production delivery was the **design, implementation, and publication of the benchmark**.
- There was also significant exploratory / strategic work around things like maturity models, possible real-time evals, and adjacent directions, but much of that remained investigative.
- Rough split of effort: approximately **2/3 consulting / leadership / strategy** and **1/3 technical**.

## Mirror Astrology

- Mirror is a **production-quality app**.
- It has **paying subscribers**, but only a small number.
- Approximate scale at the moment: **~5 monthly active subscribers** and **~5 daily active users**.
- It is fair to describe it as a real production app; do not imply significant scale.

## Kantata — Key Project Narratives

Reference material for interviews, cover letters, and resume bullets. Use these as the canonical version — prior retellings have drifted. Metrics are approximate where not explicitly noted; confirm before citing hard numbers.

### M-Bridge: Turnaround of the Integrations Platform

**Context**: M-Bridge was Kantata's integrations platform — the system connecting the Kantata SaaS to customer systems (Salesforce, HRIS, accounting, etc.). When Jack took over, it was a "dumpster fire": unreliable, flaky, frequent customer-visible failures, high on-call burden.

**What Jack did**: Led the M-Bridge team to rearchitect and stabilize the platform into a robust, scalable, reliable system.

**Result**: **~100x reduction in error rates.** Platform became a reliable foundation rather than a source of customer escalations.

### M-Bridge: Heroku → Kubernetes + RDS Migration

**Context**: M-Bridge was running on Heroku and needed to move to the company's Kubernetes + RDS stack for scale, cost, and consistency with the rest of the platform.

**What Jack did**: Led the M-Bridge team through the full migration.

**Result**: **Zero-downtime cutover.** Migrated without customer-visible impact.

### DevOps Team Rebuild After Mass Departures

**Context**: A sudden wave of departures left the DevOps team at just two engineers — and one of them was already two weeks from leaving. Critical infrastructure responsibility for the whole company was at risk.

**What Jack did**: Stepped into leadership of the DevOps team, rebuilt it from near-zero — hiring, onboarding, re-establishing team culture, documentation, on-call practices.

**Result**: Rebuilt a functional, stable team. This became the foundation for the next several initiatives below. Culture emphasized long-term thinking, strong developer relations, and sustainable on-call load.

### Rails Monolith + Services → Kubernetes Migration

**Context**: Kantata's Rails monolith and the surrounding services ecosystem were running on legacy infrastructure and needed to move to Kubernetes.

**What Jack did**: Led the DevOps team through the migration of the entire Rails monolith and all other services into Kubernetes.

**Result**: Full platform migration completed under his leadership.

### MySQL → RDS Migration (Segfaulting Stack)

**Context**: The primary MySQL stack was literally segfaulting in production — an ongoing reliability crisis.

**What Jack did**: Led the DevOps team through migration off the segfaulting stack to AWS RDS.

**Result**: Eliminated the segfault class of incidents; moved to a managed, reliable database tier.

### On-Call + Reliability Culture

**Context**: High on-call burden, frequent incidents, low team morale and retention risk across the DevOps org.

**What Jack did**: Led the DevOps team through a sustained reliability push — reducing on-call incidents and error rates, establishing team culture focused on long-term sustainability.

**Result**: Dramatically reduced on-call incidents and error rates; strong team retention, good developer relations across the engineering org. Earned a Top Performer award during this period.

### Framing Notes

- The M-Bridge turnaround (dumpster fire → 100x error reduction) is the strongest single technical-impact story.
- The DevOps rebuild is the strongest leadership / team-building story.
- Both can be woven together: "I led two teams through transformations — the integrations platform and the whole DevOps org."
- Time horizon across all of this: several years at Kantata.

## Recommendations / References Convention

Recommendations are currently kept out of the main body for ATS reasons and space discipline.

Current preference:

- If included, use a brief LinkedIn recommendations note in the footer rather than in the body.
- Avoid a large recommendations section in tailored job resumes unless specifically needed.
- `References available upon request` is generally low value and should usually be omitted.

Note: the LinkedIn recommendations line is primarily for human readers, not ATS benefit.
