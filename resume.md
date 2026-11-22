# Jack Senechal

## AI Engineer · Agentic Systems & Evaluation

**Located in Novato, CA**<br>
Phone: 415-779-2701<br>
Email: <jacksenechal@gmail.com><br>
GitHub: [github.com/jacksenechal](https://github.com/jacksenechal)<br>
LinkedIn: [linkedin.com/in/jacksenechal](https://linkedin.com/in/jacksenechal)


## Summary

AI engineer building production LLM systems: agentic delivery pipelines, evaluation frameworks, and the tools agents call. Backed by a long record running the platforms and teams that production software depends on.

- **Agentic systems in production**: designs and operates agent-driven delivery pipelines that take engineering work from spec to shipped, with the SDLC enforced in the harness rather than in a prompt.
- **LLM evaluation**: originated and co-architected an open-source evaluation framework on AISI Inspect, and built a proof-of-concept real-time classifier that scores model behavior inline at sub-100ms.
- **Tool use for agents**: ships an MCP server, and works daily on both sides of the tool-use boundary.
- **Platform and reliability depth**: built the infrastructure platform an engineering org ran on, cut a production system's error rates roughly 100x, and led a multi-year migration to cloud-native.
- **Leads and grows engineers**: close to seven years leading teams, with multiple juniors grown into senior and management roles.

## Industry Experience

### Independent Consultant · AI-Native Software Delivery
#### Client engagements | May 2026 - Present | Remote

*Scope: designs the delivery process and governance model; owns product and prioritization.*

- Running a "software factory": an agent-driven delivery pipeline where coding agents implement and a human owns the product. Production-quality output sustained over long-horizon iteration, which is where agentic development typically falls down.
- **Harness design**: the same DevOps and project-management discipline that makes human teams work, encoded into agent context and enforced by the harness. Every change passes an independent fresh-context reviewer, green CI, supply-chain scanning, and a deployment smoke check before it ships.
- **GitHub as coordination substrate**: issues, PRs, and Projects as the single ledger for agent work intake, review, and status.
- **Self-improving harness**: orchestration agents tasked with running, observing, and refining the process, converging on and shipping their own refinements within set bounds.
- **Measured agent quality**: found a quality drop-off at around 700 lines per PR (measured as agent rework before review), capped PRs at 500 and later 600 lines, and held quality while completing long-horizon tasks. Roughly 490 commits and 470+ merged PRs in about 16 weeks, with median PR open-to-merge under an hour.
- **Stack chosen for agents**: React, TypeScript, Next.js, Vercel, and Cloudflare, selected because their tooling and feedback loops give agents strong traction.
- **Product ownership**: requirements gathering, prioritization, and verifying output against deployed previews on behalf of a non-technical user base.

### Co-founder & Fractional CTO
#### Building Humane Technology | June 2025 - Present | Remote (part-time)

*Scope: technical direction and roadmap for a public benefit corporation's engineering team.*

- Originated and co-architected [HumaneBench.ai](https://humanebench.ai), an open-source LLM evaluation framework built on AISI Inspect that measures how models treat users under pressure.
- Fractional CTO to the team that built and maintains it, shaping architecture, scoring design, multi-provider support, documentation, and positioning.
- Specified, designed, and built a proof-of-concept real-time classifier that scores AI behavior against HumaneBench rubrics inline at sub-100ms, suitable for a production request path rather than batch-only evaluation.
- Designing telemetry for operational visibility and evaluation feedback loops that inform system-prompt iteration and fine-tuning.
- Built the team's publishing system: a deliberately simple Vue.js site with an agent context file so non-technical teammates could edit it, with full continuous delivery on Cloudflare (preview per PR, required review, auto-deploy on merge).
- Curating the technical roadmap: production monitoring, multi-turn evaluation, adoption maturity models.

### Co-founder & Software Engineer
#### Alchemy Astrology (formerly Mirror Astrology) | Nov 2024 - Jul 2026 | Remote

*Scope: co-founder; owned front-end and design delivery for an LLM-powered consumer subscription app.*

- Owned the front end of a production consumer subscription app: Rails views, JavaScript, HTML/CSS, Tailwind, responsive UI/UX.
- Collaborated on the back end (Rails MVC, Stripe subscription billing, SSO authentication) and partnered with co-founders on product direction and prioritization.

### Infrastructure Engineer
#### Tobiko | Mar 2024 - Oct 2024 | Remote

*Scope: cloud platform serving production customer workloads.*

- Architected and implemented a cloud platform serving customer workloads at an early-stage startup. Python, Pulumi, GCP, GKE, Cloud Run, Helm.
- Built CI/CD primitives the rest of engineering used: mono-repo conditional workflows, workload identity federation, continuous delivery.
- Owned build-vs-buy for support and incident response: selected incident.io, built a Slack support tool from scratch in Python, and onboarded staff and customers onto it.

### Engineering Manager / Principal Software Engineer
#### Mavenlink / Kantata | Apr 2017 - Dec 2023 | San Francisco, CA

*Scope: hired as a Senior Software Engineer, leading teams within a few months, and promoted to Principal for the infrastructure turnaround. Led two engineering teams for close to seven years, including the shared infrastructure platform relied on by every engineering team in the company.*

- **Internal Infrastructure Platform** (4 yrs): Built a new team from scratch whose product was the platform the entire engineering org built on, and ran it as a service org with internal customers: turned recurring one-off asks into shared primitives and self-serve tooling so teams could ship without waiting on us. Owned the roadmap while staying hands-on in code, architecture, and review.
- Led the multi-year modernization of that platform from legacy infrastructure to cloud-native: the whole Rails monolith and its service ecosystem onto Kubernetes with Terraform and Ansible, the primary MySQL database onto RDS, and HashiCorp Vault stood up as an internal secrets service. Cut on-call incidents from roughly weekly to roughly quarterly.
- Rebuilt the team after mass departures: inherited a one-person DevOps team and rebuilt hiring, onboarding, documentation, and on-call practice into a stable team with strong developer relations.
- **M-Bridge Integration Platform** (2.5 yrs): Took over an unreliable agent-based integration platform connecting the SaaS to customer systems (Salesforce, HRIS, accounting) and led its rearchitecture into a dependable one. Cut error rates roughly 100x by instrumenting the system and fixing what the data pointed at. Executed a zero-downtime migration from Heroku to Google Cloud (GKE and Cloud SQL).
- Grew multiple junior engineers into senior SWE and Engineering Manager roles; led interviewing and hiring. Top Performer Award, 2021.

### Lead Developer, Co-founder
#### Pegg | 2014 - 2017 | San Francisco, CA

- Designed, architected, and built a cross-platform mobile app from scratch for iOS and Android: Node.js backend, JavaScript frontend with Redux, Firebase real-time systems, CI/CD to AWS/CloudFront via CircleCI. Established the engineering workflow from nothing and co-led product strategy and launch.

### Earlier Career (2001 - 2014)

Full-stack consulting and lead roles in Ruby on Rails, Node.js, and D3. Introduced automated testing and CI at OnForce. Architected the initial release of mynewsletterbuilder.com and built its dev team at JBA Network.

## Open Source Projects

**Scan MCP** (2024 - Present): MCP server giving AI agents control of document scanners, exposing scanner discovery and capture as tools an agent calls. Privacy-first architecture, JSON Schema validation, stdio and HTTP transports so it runs locally or remotely. TypeScript/Node.js. [github.com/jacksenechal/scan-mcp](https://github.com/jacksenechal/scan-mcp)

**HumaneBench** (2024 - Present): Open-source LLM evaluation framework built on AISI Inspect. See Building Humane Technology above. Python. [github.com/buildinghumanetech/humanebench](https://github.com/buildinghumanetech/humanebench)

## Skills

- **AI/LLM**: agentic coding systems and harness design, LLM evaluation (AISI Inspect, rubric-based scoring, real-time classification), MCP servers and tool use, multi-provider evaluation design, prompt engineering, context augmentation, Claude Code and orchestrated subagents, evaluation telemetry.
- **Languages & Frameworks**: Python, TypeScript, JavaScript, Node.js, React, Vue, Next.js, Ruby on Rails, Bash.
- **Infrastructure & CI/CD**: AWS, GCP, Kubernetes, Docker, Terraform, Pulumi, Ansible, Helm, GitHub Actions, CircleCI, Vercel, Cloudflare, infrastructure as code, automated testing, TDD, supply-chain security scanning.
- **Back-end & Data**: API design, microservices, distributed systems, PostgreSQL, MySQL, MongoDB, Redis, observability and instrumentation.
- **Product & Leadership**: roadmap ownership, product discovery with users, prioritization, team building, hiring, coaching and mentoring, stakeholder engagement.

## Education

### BA in Mathematics, minor in Computer Science
#### University of North Carolina at Asheville | May 2003

- Graduated with distinction in Mathematics. Undergraduate research in 4D fractals.

## Recommendations

"Jack is an exceptional engineer and leader. He strives to deeply understand the technology he's working on while remaining cognizant of the socio-technical components that may be a factor in any project. He's thorough, detail-oriented, and outcome-oriented, which means the solutions he architects, builds, and collaborates on come out better. Jack also strives to be at the forefront of new technology and assess how he can leverage it. Newer tech like GenAI can be complex and ever-evolving, and Jack is not one to back down but step up and embrace. He does all this with a strong team mentality, is a phenomenal team player, and can effectively delegate to help lift others' skill sets."

*— Brandon Clifford, Director of DevOps, Kantata*

"Jack has had quite a profound impact on my career. As a young engineer, I was fortunate enough to work with Jack as my coach. He served as a great mentor, helping me build both technical and professional skills and forming me into the engineer that I am today. Throughout our time together, Jack was caring and invested in helping me set goals and develop my career. His mentorship was a key factor in elevating myself from an incoming Junior Engineer to an Engineering Manager. Jack has a great curiosity and a strong set of technical capabilities that allow him to serve as a great example for others and a key contributor to any team!"

*— Wesley Morlock, Engineering Director, Kantata*

"Jack is a fantastic engineer always ready to help solve problems and more importantly, teach you how to solve them. He guided me and my team through a bunch of challenging GitOps situations with patience and kindness, leading by example. Always diligent with his work, willing to roll up his sleeves to get things done and find creative solutions."

*— Cesar Palafox Garza, Principal Software Engineer, Kantata*

[See additional recommendations on LinkedIn](https://linkedin.com/in/jacksenechal)
