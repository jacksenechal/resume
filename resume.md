# Jack Senechal

## Product Engineer · Full-Stack Generalist

**Novato, CA** · 415-779-2701 · <jacksenechal@gmail.com><br>
GitHub: [github.com/jacksenechal](https://github.com/jacksenechal) · LinkedIn: [linkedin.com/in/jacksenechal](https://linkedin.com/in/jacksenechal)

## Summary

Full-stack product engineer with a strong record of shipping production software and infrastructure, most of it at startups and as a founder. No big-company detour.

- **Platform architect** for internal tools other people build on: shared infrastructure, integration middleware, and developer-facing primitives with real internal customers.
- **Team of one, with leadership chops.** Comfortable taking products from idea to shipped across backend, frontend, and infrastructure, with the product judgment to know what is worth building.
- **Owns outcomes, not tickets.** A rescuer of burning platforms, at home with incomplete information, able to take a room of stakeholders and engineers to clarity.
- Every role here has shipped **user-facing experience**, for technical and non-technical audiences alike.

## Industry Experience

### Independent Consultant · AI-Native Software Delivery
#### Client engagements | May 2026 - Present | Remote

- Run "software factories": agent-driven delivery pipelines that carry engineering work from spec to shipped, human in the product seat. **Speed without fragility**: production-quality output over long-horizon iteration, where agentic development typically falls down.
- **Core thesis**: the same DevOps and project-management discipline that makes human teams work is the necessary and sufficient foundation for agent teams, encoded into the harness and context.
- **GitHub as coordination substrate**: issues, PRs, and Projects as the single ledger. Harness-enforced SDLC (independent fresh-context reviewer, green CI, supply-chain scanning, deployment smoke check) so agents move fast without breaking things.
- **Self-improving harness**: orchestration agents run, observe, and refine the process, converging on and shipping their own refinements.
- Chose **React, TypeScript, and Next.js** stack: their tooling and feedback loops are very tractable for agents to work in.
- **Product ownership**: defining and prioritizing the work, and verifying against deployed previews on behalf of a non-technical user base.
- **Matching approach to the work**: a prototype is far faster driving an agent directly; the factory earns its keep on production systems, where the industry is converging.

### Co-founder & Fractional CTO
#### Building Humane Technology | June 2025 - Present | Remote (part-time)

- Originated and co-architected [HumaneBench.ai](https://humanebench.ai), an open-source AI evaluation framework built on AISI Inspect. **Python.**
- Fractional CTO to the team that built it into a published, externally usable product, shaping architecture, scoring design, multi-provider support, documentation, and positioning.
- Built a low-latency proof-of-concept classifier scoring model behavior against HumaneBench rubrics inline at **sub-100ms**, suitable for a production request path rather than batch only.
- Designs telemetry for operational visibility and evaluation feedback loops informing system-prompt iteration and fine-tuning. Owns the technical roadmap: production monitoring, multi-turn evaluation, adoption maturity models.

### Co-founder & Software Engineer
#### Alchemy Astrology (formerly Mirror Astrology) | Nov 2024 - Jul 2026 | Remote

- Owned the front end of a production consumer subscription app: Rails views, JavaScript, HTML/CSS, Tailwind, responsive UI/UX.
- Led design and UX delivery: worked directly with freelance designers, translated Figma into the Rails framework. Collaborated on the back end: Rails MVC, Stripe subscription billing, SSO authentication.
- Made product and prioritization calls with co-founders: roadmap, scope, what to ship next.

### Infrastructure Engineer
#### Tobiko | Mar 2024 - Oct 2024 | Remote

- Architected and implemented a cloud platform serving customer workloads at an early-stage startup. **Python**, Pulumi, GCP, GKE, Cloud Run, Helm.
- Built CI/CD primitives the rest of engineering used: mono-repo conditional workflows, workload identity federation, continuous delivery.
- Owned build-vs-buy for support and incident response: selected incident.io for incident management; after support tooling review found nothing that handled Slack-based support cleanly, built the Slack support agent from the ground up in Python and onboarded teammates and customers onto it.

### Principal Software Engineer / Engineering Manager
#### Mavenlink / Kantata | Apr 2017 - Dec 2023 | San Francisco, CA

- **M-Bridge Integration Platform** (2 yrs): Took over an unreliable agent-based integration platform connecting the SaaS to customer systems (Salesforce, HRIS, accounting) and led its rearchitecture into a dependable one. **Cut error rates roughly 100x** by instrumenting the system and fixing what the data pointed at. Executed a **zero-downtime migration** from Heroku to Kubernetes and RDS, including relational, document, and cache stores.
- **Internal Infrastructure Platform** (4 yrs): Built a new team from scratch whose product was the platform the entire engineering org built on. Ran it as a service org with internal customers: consulted with teams on their workflows, triaged requests, and turned recurring one-off asks into shared primitives and self-serve tooling so teams could ship without waiting on us. Owned the roadmap while staying hands-on in code, architecture, and review. Migrated a large legacy Rails monolith and its service ecosystem to cloud-native infrastructure (Terraform, Ansible, Kubernetes).
- Rebuilt the team after mass departures: inherited a two-person DevOps team with one member two weeks from leaving, rebuilt hiring, onboarding, documentation, and on-call practice into a stable team with strong developer relations.
- Led a transition team that took ownership of the BI/analytics pipeline and migrated it to Kubernetes.
- Shipped **React** features in the customer-facing product and worked in its **Redux** state management, alongside the platform and infrastructure work.
- Grew multiple junior engineers into senior SWE and Engineering Manager roles; led interviewing and hiring. **Top Performer Award, 2021.**

### Lead Developer, Co-founder
#### Pegg | 2014 - 2017 | San Francisco, CA

- Designed, architected, and built a cross-platform mobile app from scratch for iOS and Android. Node.js backend, JavaScript frontend with **Redux** state management, Firebase real-time systems, CI/CD to AWS/CloudFront via CircleCI.
- Established the engineering workflow from nothing (pair programming, automated testing, CI, rapid deployment) and co-led product strategy, monetization, and launch planning.

### Earlier Career (2001 - 2014)

Full-stack consulting and lead roles in Ruby on Rails, Node.js, and D3 (OpenTest Pro, Turnbull & Asser e-commerce). Introduced automated testing and CI at OnForce. Architected the initial release of mynewsletterbuilder.com and built its dev team at JBA Network.

## Open Source Projects

**Scan MCP** (2024 - Present): MCP server giving AI agents control of document scanners. Privacy-first architecture, device discovery, JSON Schema validation, stdio and HTTP transports. **TypeScript/Node.js.** [github.com/jacksenechal/scan-mcp](https://github.com/jacksenechal/scan-mcp)

**HumaneBench** (2024 - Present): Open-source LLM evaluation framework built on AISI Inspect. See Building Humane Technology above. **Python.** [github.com/buildinghumanetech/humanebench](https://github.com/buildinghumanetech/humanebench)

## Skills

- **Languages & Frameworks**: Python, TypeScript, JavaScript, React, Vue, Node.js, Ruby on Rails, Bash, HTML, CSS, Tailwind.
- **Front-end**: responsive design, UI/UX collaboration with designers, Figma handoff.
- **Back-end & Data**: API design, microservices, distributed systems, PostgreSQL, MySQL, MongoDB, Redis, Stripe, SSO/auth.
- **AI/LLM**: LLM evaluation frameworks (AISI Inspect), MCP servers, chatbot development, prompt engineering, context augmentation, agentic coding workflows.
- **Infrastructure & CI/CD**: AWS, GCP, Kubernetes, Docker, Terraform, Pulumi, Ansible, Helm, GitHub Actions, CircleCI, infrastructure as code, automated testing, TDD.
- **Product**: Roadmap ownership, product discovery with users, prioritization, scope negotiation, cross-functional collaboration.

## Education

### BA in Mathematics, minor in Computer Science
#### University of North Carolina at Asheville | May 2003

Graduated with distinction in Mathematics. Undergraduate research in 4D fractals.
