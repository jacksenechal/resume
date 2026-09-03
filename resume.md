# Jack Senechal

## Systems Engineering Manager · Infrastructure & Reliability

**Located in Novato, CA**<br>
Phone: 415-779-2701<br>
Email: <jacksenechal@gmail.com><br>
GitHub: [github.com/jacksenechal](https://github.com/jacksenechal)<br>
LinkedIn: [linkedin.com/in/jacksenechal](https://linkedin.com/in/jacksenechal)

## Summary

Hands-on infrastructure leader with **6+ years leading teams**, and still in the terminal alongside them. Player/coach by preference: roadmap, hiring, and on-call design in one hand, architecture and code review in the other.

- **Rebuilt a DevOps team** from two engineers after mass departures: hiring, onboarding, documentation, and sustainable on-call practices, then drove the reliability push that cut on-call incidents and earned a **Top Performer Award, 2021**.
- **Fleet and configuration management**: moved a large legacy Linux estate to Infrastructure-as-Code with **Ansible, Terraform, and Kubernetes**, replacing hand-built servers with reproducible, drift-resistant state.
- **Reliability record**: rearchitected an unreliable production platform for **~100x error reduction**, and led a **zero-downtime** migration of it to Kubernetes and RDS.
- **Operational rigor**: monitoring and alerting, incident response and postmortems, change control, and CI/CD gates as the default way work ships.
- **AI-native practice**: operates agent-driven delivery pipelines gated by review, CI, and supply-chain scanning, a live view of where automation actually pays.

## Professional Experience

### Independent Consultant · AI-Native Software Delivery
#### Client engagements | May 2026 - Present | Remote

- Designs and runs **agent-driven delivery pipelines** that carry engineering work from spec to shipped, with the human in the product seat.
- **Harness-enforced SDLC**: every change gated by an independent fresh-context reviewer, green CI, **supply-chain scanning**, and a deployment smoke check. The operating thesis is that the DevOps discipline that makes human teams work is what makes agent teams work, and that anything merely instructed rather than enforced will drift.
- GitHub as the single durable ledger for issues, PRs, and board state, with board state **derived from CI and PR reality** rather than maintained by hand.

### Co-founder & Fractional CTO
#### Building Humane Technology | June 2025 - Present | Remote (part-time)

- **Originated and co-architected [HumaneBench.ai](https://humanebench.ai)**, an open-source AI evaluation framework built on AISI Inspect. **Python.**
- Built a **low-latency proof-of-concept classifier** scoring model behavior against HumaneBench rubrics inline at **sub-100ms**, fast enough to sit in a production request path rather than run only in batch.
- Designed **telemetry for operational visibility** and the feedback path carrying evaluation output back into system-prompt iteration.

### Co-founder & Software Engineer
#### Alchemy Astrology (formerly Mirror Astrology) | Nov 2024 - Jul 2026 | Remote

- Owned front-end and design/UX delivery for a production consumer subscription app: Ruby on Rails views, JavaScript, Tailwind, responsive UI.
- Collaborated on back-end work: Stripe billing integration, SSO authentication, Rails MVC.

### Infrastructure Engineer
#### Tobiko | Mar 2024 - Oct 2024 | Remote

- Designed, built, and operated a cloud platform running production customer workloads, with reliability, security, and operational excellence as the standard.
- Operated **Kubernetes**-based services with observability and incident response practices attached, and implemented **infrastructure as code** for consistent, repeatable deployments.
- Built CI/CD patterns including mono-repo conditional workflows, **workload identity federation** for credential-free access, and continuous delivery.
- Stood up a Slack-based customer support and **incident response** workflow; onboarded teammates and customers onto it.
- Python, Pulumi, GCP, GKE, Cloud Run, CircleCI, Helm.

### Engineering Manager / Principal Software Engineer
#### Mavenlink / Kantata | Apr 2017 - Dec 2023 | San Francisco, CA

- **Infrastructure Platform / DevOps** (4 years): Took over a DevOps team reduced to two engineers by mass departures and rebuilt it: recruiting, onboarding, documentation practice, and an **on-call rotation the team could sustain**. Led the organization's DevOps culture transformation as change agent and technical authority across engineering. Owned roadmap stewardship, requirements triage, and priority management while **staying hands-on with coding, architecture, and code review**.
- **Fleet modernization**: Transitioned a large legacy codebase and its Linux server estate to cloud-native, **Infrastructure-as-Code tooling (Terraform, Ansible, Kubernetes)**, standardizing provisioning, patching, and configuration management. Led the migration of the Rails monolith and surrounding services into Kubernetes, and the migration of a **segfaulting production MySQL stack onto managed RDS**, eliminating a whole class of incidents.
- **M-Bridge Integration Platform** (2 years): Led the team that stabilized and scaled Kantata's integration platform, an agent-based system doing multi-system data orchestration. Established the **operational metrics, monitoring, and alerting** that took it from frequent customer-visible failures to **~100x fewer errors and incidents**. Executed a **zero-downtime migration to Kubernetes**, including relational, document, and cache datastores.
- **Reliability and on-call culture**: Drove a sustained push that dramatically reduced on-call incident volume and error rates. Strong retention and good developer relations across the engineering org came out of it.
- **BI Data Pipeline** (3 months): Led a transition team that took ownership of the analytics data pipeline and migrated it to Kubernetes.
- **People and cross-functional impact**: **Grew multiple junior engineers into senior SWE and Engineering Manager roles**, and mentored engineers across teams. Led interviewing and hiring. Partnered with product, security, and application teams on shared infrastructure and organizational change.

### Lead Developer, Co-founder
#### Pegg | 2014 - 2017 | San Francisco, CA

- Designed, architected, and built a cross-platform mobile app from scratch. Node.js backend, Firebase real-time systems, CI/CD to AWS/CloudFront via CircleCI.
- Established the engineering workflow: pair programming, automated testing, continuous integration, and rapid deployment.

### Earlier Career (2001 - 2014)

- **Consultant & Entrepreneur** (2008 - 2014): Founded OpenTest Pro (automated testing education). Built an e-commerce ordering system for Turnbull & Asser shirtmakers. Full-stack consulting in Ruby on Rails and Node.js.
- **Web Developer, OnForce, Inc** (2006 - 2007): Introduced automated testing and CI. Built a comprehensive API test suite. Integrated the platform with Salesforce APIs.
- **Development Lead, JBA Network** (2003 - 2006): Lead programmer and project manager for mynewsletterbuilder.com. Architected the initial release, then built and scaled the development team.

## Selected Projects

### Scan MCP (2024 - Present)

MCP server for scanner automation and document digitization. Privacy-first architecture with device discovery, JSON Schema validation, and both local stdio and network HTTP transports. TypeScript/Node.js. [github.com/jacksenechal/scan-mcp](https://github.com/jacksenechal/scan-mcp)

### HumaneBench (2024 - Present)

Evaluation framework for measuring human-friendly behavior in AI assistants, built on AISI Inspect. Multiple LLM providers, extensible scenario datasets. Python. [github.com/buildinghumanetech/humanebench](https://github.com/buildinghumanetech/humanebench)

## Skills

- **Systems & Infrastructure**: Linux systems administration, fleet and configuration management, Ansible, Terraform, Kubernetes, Docker, Helm, Pulumi, AWS, Google Cloud Platform, capacity planning, patching and upgrade cadence.
- **Reliability & Operations**: Monitoring and alerting, log aggregation, on-call rotation design, incident response and postmortems, change control, disaster recovery, zero-downtime migration.
- **Networking & Services**: DNS, TLS and certificate management, load balancing, HTTP and TCP/IP troubleshooting, service-to-service authentication.
- **Security**: Access management, SSO, secrets and credential handling, workload identity federation, supply-chain scanning, hardening and posture improvement.
- **Automation & Scripting**: Bash, Python, JavaScript/TypeScript, Ruby, CI/CD (GitHub Actions, CircleCI), Infrastructure as Code, internal tooling and API development.
- **Data Stores**: PostgreSQL, MySQL, RDS, MongoDB, Redis.
- **Leadership**: Team building, hiring and onboarding, coaching and mentoring, performance and career development, roadmap ownership, cross-functional collaboration, vendor and stakeholder communication, change management.

## Education

### BA in Mathematics, minor in Computer Science
#### University of North Carolina at Asheville | May 2003

- Graduated with distinction in Mathematics. Undergraduate research in 4D fractals.

## Recommendations

"Jack is **an exceptional engineer and leader**. He strives to **deeply understand the technology** he's working on while remaining cognizant of the socio-technical components that may be a factor in any project. He's thorough, detail-oriented, and outcome-oriented, which means **the solutions he architects, builds, and collaborates on come out better**. He does all this with a **strong team mentality**, is a phenomenal team player, and can **effectively delegate to help lift others' skill sets**."

*— Brandon Clifford, Director of DevOps, Kantata*

"Jack has **had quite a profound impact on my career**. As a young engineer, I was fortunate enough to work with Jack as my coach. He served as a great mentor, helping me build both technical and professional skills and **forming me into the engineer that I am today**. **His mentorship was a key factor in elevating me from an incoming Junior Engineer to an Engineering Manager**."

*— Wesley Morlock, Engineering Manager, Kantata*

"Jack is a fantastic engineer always ready to **help solve problems and more importantly, teach you how to solve them**. He guided me and my team through a bunch of challenging GitOps situations with patience and kindness, leading by example. Always diligent with his work, willing to roll up his sleeves to get things done and **find creative solutions**. Everyone would be lucky to have someone like him in their teams!"

*— Cesar Palafox Garza, Principal Software Engineer, Kantata*

[See additional recommendations on LinkedIn](https://linkedin.com/in/jacksenechal)
