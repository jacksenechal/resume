# Jack Senechal

## Product Engineer · Full-Stack Generalist

**Located in Novato, CA**<br>
Phone: 415-779-2701<br>
Email: <jacksenechal@gmail.com><br>
GitHub: [github.com/jacksenechal](https://github.com/jacksenechal)<br>
LinkedIn: [linkedin.com/in/jacksenechal](https://linkedin.com/in/jacksenechal)

## Summary

- **Full-stack product engineer, 20+ years shipping production software**, most of it at startups and as a founder. No big-company detour.
- **Builds the platform behind the feature request.** Specializes in internal tools and platforms that other people build on: shared infrastructure, integration middleware, and developer-facing primitives with real internal customers.
- **Operates as a team of one when the job calls for it.** Four founding ventures, taking products from idea to shipped and running across backend, frontend, and infrastructure.
- **Works directly with users.** Ran internal platform teams as a service organization, consulting with engineers and stakeholders, triaging requests, and turning recurring one-offs into general capabilities.
- **Owns outcomes, not tickets.** Roadmap ownership, product and prioritization calls, and accountability for whether the thing actually solved the problem.
- **Builds the machine that builds the software.** Designs and operates agent-driven delivery pipelines that ship production code end to end, and builds with LLMs directly (evaluation frameworks, MCP servers, chat products).

## Industry Experience

### Independent Consultant — AI-Native Software Delivery
#### Client engagements | May 2026 - Present | Remote

- **Build and operate "software factories"**: agent-driven delivery pipelines that take engineering work from spec to shipped, with the human in the product seat. Two persistent orchestrating agent sessions delegate implementation to cheaper-model subagents, each isolated in its own **git worktree and database**.
- **Delivered a production web app this way** (Next.js, Payload CMS, Postgres, Vercel): **~261 merged PRs across 190 issues in 13 weeks**, with roughly three-quarters of commits agent-produced behind automated and human review gates.
- **Built the coordination substrate on GitHub itself** (issues, PRs, and Projects as the single ledger), including scheduled automation that **derives board state from PR, CI, and label reality** instead of relying on agents to remember to update it, after observing that instruction-based state tracking reliably drifts.
- **Engineered a lifecycle hook that structurally prevents lost work**, refusing to let an agent session end while any dispatched worktree holds uncommitted or unpushed changes. Diagnosed why the first version missed the real failure population and rebuilt it with a staleness heuristic separating abandoned lanes from in-flight ones.
- **Designed the concurrency model**: one worktree per task, stacked PR trains for multi-PR features, a correct procedure for GitHub's squash-merge diff-base staleness, and **database migration governance** (mandatory committed migrations, a CI gate catching silent no-op migrations, and a recovery procedure for concurrent-migration snapshot drift) built in response to real incidents.
- Hold the **product role by design**: define and prioritize the work, QA against deployed previews, and own the one human sign-off gate before anything ships to users.

### Co-founder & Fractional CTO
#### Building Humane Technology | June 2025 - Present | Remote (part-time)

- **Originated the concept for [HumaneBench.ai](https://humanebench.ai)** and co-architected it: an open-source AI evaluation framework built on AISI Inspect. **Python.**
- Act as **fractional CTO to the team** that built it out to a published, externally usable product, shaping architecture, scoring design, and multi-provider support, and guiding documentation and positioning.
- Extending the framework toward **real-time evaluation**: specified and designed a **low-latency proof-of-concept classifier**, built in collaboration with coding agents, that scores model behavior against HumaneBench rubrics inline at **sub-100ms** and can sit in a production request path rather than run only in batch.
- Translated qualitative behavioral rubrics into **structured, trainable signal definitions**, and designed the **operational visibility metrics** and automated feedback path carrying evaluation output back into **system-prompt iteration and model fine-tuning**.
- Own **product direction and roadmap**: production monitoring, multi-turn evaluation, and adoption maturity models.

### Co-founder & Software Engineer
#### Alchemy Astrology (formerly Mirror Astrology) | Nov 2024 - Jul 2026 | Remote

- **Owned the front end** of a production consumer subscription app: Rails views, JavaScript, HTML/CSS, Tailwind, and responsive UI/UX.
- **Led design and UX delivery**: worked directly with freelance designers, then translated their Figma designs into the Rails framework.
- Collaborated on the back end: Rails MVC, Stripe subscription billing, SSO authentication.
- Made product and prioritization calls with co-founders: roadmap, scope, what to cut, what to ship next.

### Infrastructure Engineer
#### Tobiko | Mar 2024 - Oct 2024 | Remote

- Architected and implemented a cloud platform serving customer workloads at an early-stage startup. **Python**, Pulumi, GCP, GKE, Cloud Run, Helm.
- Built CI/CD primitives the rest of engineering used: mono-repo conditional workflows, workload identity federation, continuous delivery.
- **Owned the build-vs-buy decision** for customer support and incident response. Selected incident.io for incident management; after a thorough review of support tooling turned up nothing that handled Slack-based support cleanly, **built the Slack support agent from the ground up in Python**, then onboarded teammates and customers onto it.

### Principal Software Engineer / Engineering Manager
#### Mavenlink / Kantata | Apr 2017 - Dec 2023 | San Francisco, CA

- **M-Bridge Integration Platform** (2 years): Took over an unreliable agent-based integration platform connecting the SaaS to customer systems (Salesforce, HRIS, accounting) and led its rearchitecture into a dependable one. **Cut error rates roughly 100x** by instrumenting the system and fixing what the data actually pointed at. Executed a **zero-downtime migration** from Heroku to Kubernetes and RDS, including relational, document, and cache stores.
- **Internal Infrastructure Platform** (4 years): Built a new team from scratch whose product was the platform the entire engineering organization built on. Ran it as a service org with internal customers: consulted with teams on their workflows, triaged requests, and **reduced recurring one-off asks into shared primitives and self-serve tooling** so teams could ship without waiting on us. Owned the roadmap while staying hands-on in code, architecture, and review. Migrated a large legacy Rails monolith and its service ecosystem to cloud-native infrastructure (Terraform, Ansible, Kubernetes).
- **Rebuilt the team after mass departures**: inherited a two-person DevOps team with one member two weeks from leaving, and rebuilt hiring, onboarding, documentation, and on-call practice from near zero into a stable team with strong developer relations.
- **BI Data Pipeline** (3 months): Led a transition team that took ownership of the analytics pipeline and migrated it to Kubernetes.
- **Grew multiple junior engineers into senior SWE and Engineering Manager roles**; led interviewing and hiring. **Top Performer Award, 2021.**

### Lead Developer, Co-founder
#### Pegg | 2014 - 2017 | San Francisco, CA

- Designed, architected, and built a cross-platform mobile app from scratch for iOS and Android. Node.js backend, JavaScript frontend, Firebase real-time systems, CI/CD to AWS/CloudFront via CircleCI.
- Established the engineering workflow from nothing: pair programming, automated testing, continuous integration, rapid deployment.
- Co-led product strategy, monetization, and launch planning.

### Earlier Career (2001 - 2014)

- **Consultant & Entrepreneur** (2008 - 2014): Founded OpenTest Pro (automated testing education). Built an e-commerce ordering system for Turnbull & Asser shirtmakers. Full-stack consulting in Ruby on Rails, Node.js, and D3 data visualization, with rapid prototyping and direct client delivery.
- **Web Developer, OnForce, Inc** (2006 - 2007): Introduced automated testing and CI. Built a comprehensive API test suite. Integrated the platform with Salesforce APIs.
- **Development Lead, JBA Network** (2003 - 2006): Lead programmer and project manager for mynewsletterbuilder.com. Architected the initial release, then built and scaled the development team.

## Open Source Projects

### Scan MCP (2024 - Present)

MCP (Model Context Protocol) server that gives AI agents control of document scanners. Privacy-first architecture with smart device discovery, JSON Schema validation, and both local stdio and network HTTP transports. **TypeScript/Node.js.**

[github.com/jacksenechal/scan-mcp](https://github.com/jacksenechal/scan-mcp)

### HumaneBench (2024 - Present)

Evaluation framework for measuring human-friendly behavior in AI assistants, built on AISI Inspect. Tests AI responses across humane technology principles including loneliness, mental health, transparency, and privacy. Multi-provider LLM support with extensible scenario datasets. **Python.**

[github.com/buildinghumanetech/humanebench](https://github.com/buildinghumanetech/humanebench)

## Skills

- **Core**: Python, TypeScript, JavaScript, React, Node.js, Ruby on Rails, Bash.
- **Front-end**: React, Vue, HTML, CSS, Tailwind, responsive design, UI/UX collaboration with designers.
- **Back-end & Data**: API design, microservices, distributed systems, PostgreSQL, MySQL, MongoDB, Redis, Stripe, SSO/auth.
- **AI/LLM**: LLM evaluation frameworks (AISI Inspect), MCP (Model Context Protocol) servers, chatbot development, prompt engineering, context augmentation, agentic coding workflows.
- **Infrastructure**: AWS, Google Cloud Platform, Kubernetes, Docker, Terraform, Pulumi, Ansible, Helm.
- **CI/CD & Practice**: GitHub Actions, CircleCI, automated testing, TDD, infrastructure as code, rapid prototyping.
- **Product**: Roadmap ownership, product discovery with users, prioritization, scope negotiation, cross-functional collaboration with design and business stakeholders.

## Education

### BA in Mathematics, minor in Computer Science
#### University of North Carolina at Asheville | May 2003

- Graduated with distinction in Mathematics. Undergraduate research in 4D fractals.

## Recommendations

"Jack is **an exceptional engineer and leader**. He strives to **deeply understand the technology** he's working on while remaining cognizant of the socio-technical components that may be a factor in any project. He's thorough, detail-oriented, and outcome-oriented, which means **the solutions he architects, builds, and collaborates on come out better**. Jack also strives to be at the forefront of new technology and assess how he can leverage it. He does all this with a **strong team mentality**, is a phenomenal team player, and can **effectively delegate to help lift others' skill sets**."

*— Brandon Clifford, Director of DevOps, Kantata*

"Jack is a fantastic engineer always ready to **help solve problems and more importantly, teach you how to solve them**. He guided me and my team through a bunch of challenging GitOps situations with patience and kindness, leading by example. Always diligent with his work, willing to roll up his sleeves to get things done and **find creative solutions**. Everyone would be lucky to have someone like him in their teams!"

*— Cesar Palafox Garza, Principal Software Engineer, Kantata*

[See additional recommendations on LinkedIn](https://linkedin.com/in/jacksenechal)
