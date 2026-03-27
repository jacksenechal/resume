# Interview Prep: Phoenix Technologies — Engineering Lead

## Quick Company Brief

**Phoenix Technologies** is "the operating system of performance commerce" — a unified platform for D2C (direct-to-consumer) merchants covering checkout, payments, subscriptions, analytics, and LTV optimization.

- **Founded:** October 2023 by **Kevin Zhang** (serial D2C entrepreneur, $150M+ in bootstrapped ecommerce revenue, Vanderbilt '18, turned down McKinsey)
- **Growth:** $10M ARR in ~15 months. 35% month-over-month growth since May 2024. On track for $350M+ GMV in 2025.
- **Funding:** $5M round (November 2025). Appears bootstrapped/lean prior to that.
- **Size:** ~27-43 employees. Small, fast, high-output team.
- **Location:** Miami, FL HQ. Engineering is 100% remote.
- **Tech stack (from job listing):** TypeScript, Node.js, React, NestJS, AWS, Kubernetes, Docker

### What They Actually Build
- **Phoenix Payments:** Smart payment routing (by BIN, geography, card type), 90%+ auth rates, decline recovery via AI. Supports Stripe, Shopify Payments, Apple Pay, Google Pay, PayPal, Airwallex, NMI, and 10+ processors.
- **Phoenix Conversions:** Drag-and-drop funnel builder, custom checkout flows, A/B testing, dynamic urgency/personalization elements. Claim: "3X faster checkout."
- **Phoenix MRR:** Subscription management — pause, reactivation, instant refunds, unified customer records, automated retention workflows.
- **Analytics Dashboard:** Real-time revenue tracking, LTV forecasting by cohort, churn detection.

### Core Value Prop
"Make 20% more money with every checkout." They help merchants who are already doing $1.5M+ GMV optimize conversion, payment approval rates, and recurring revenue. The Costco/Sam's Club model for D2C — turning one-time buyers into high-margin subscription members.

### Target Customers
D2C merchants: dropshipping, ecommerce, nutraceuticals, subscription businesses. They host exclusive invite-only events for "$5M+/year founders."

---

## Key People

### Kevin Zhang — Founder & CEO
- Moved to US at age 4 (Chinese immigrant family). Vanderbilt '18 (Economics + Political Science, Corporate Strategy minor).
- Declined McKinsey to do ecommerce. Built a Shopify business to $150M+ in sales. Pioneered subscription strategies generating $60M in revenue.
- Vision: Replicate Costco/Sam's Club membership model for D2C retailers.

### Stas Filippov — CTO
- Former VP of Engineering at Skillshare (scaled to millions of users, 99.99% uptime).
- Staff Engineer at Step (mobile banking — microservices powering a fintech app).
- Head of Technology at iKobo (international person-to-person money transfers — **payments background**).
- Co-Founder at Radnology (financial services tech).
- **Key insight:** Stas has deep payments/fintech engineering background. He'll likely be the technical bar-raiser in later rounds.

### Tim Schulz — CPO
- 15+ years in global commerce. Leadership roles at BigCommerce, Magento, and VTEX (all major ecommerce platforms).
- Managed products handling billions in annual GMV.

### Tony Kochhar — Chief People Officer *(He reached out to you)*
- 15+ years in talent strategy at high-growth tech firms.
- Contributed to $900M+ in startup exits.
- Philosophy: "AI is not replacing meaningful human connection, it's making it more valuable." Values relationship depth over network size.
- Hofstra University. Bilingual (English/Hindi).
- Writes about AI careers, hiring trends, agentic AI.

### Sona Bhatia — Recruiter *(Your interviewer today)*
- Talent Acquisition specialist.
- LinkedIn profile wasn't fully accessible, but she's the TA coordinator for engineering hires.

---

## Your Interview: What to Expect

This is a **recruiter screen** — likely 30 minutes. Sona will be evaluating:
1. **Fit check:** Do your experience and interests align with the role?
2. **Motivation:** Why Phoenix? Why now?
3. **Logistics:** Compensation expectations, availability, remote work setup, visa status (they can't sponsor H1B — not relevant for you).
4. **Culture fit:** Are you the "no fluff, move fast" type?

They reached out to *you* on LinkedIn, so you're already validated. This is more about mutual fit than proving yourself.

---

## What to Lean Into (Your Strengths for This Role)

### 1. Kantata: The Crown Jewel Experience
This is your strongest card. 6+ years, dual EM/Principal Engineer role. Hit every bullet in their job listing:
- **Led multiple pods/teams** — Operations team (4 years), M-Bridge team (2 years), Insights team. You recruited, built, and scaled teams from scratch.
- **Stayed hands-on while leading** — You coded, architected, and collaborated on mission-critical projects while managing teams. This is *exactly* what they want: "day to day coding role + leading a small pod."
- **Quantifiable impact** — 100x reduction in errors/incidents on M-Bridge. Zero-downtime Kubernetes migrations. Top Performer Award 2021.
- **Cloud-native, distributed systems** — Kubernetes migrations, microservices, Infrastructure as Code. Maps directly to their AWS/K8s/Docker requirements.
- **DevOps culture transformation** — Led organizational shift toward DevOps. This signals you can shape engineering culture, not just write code.
- **Cross-functional collaboration** — Mentoring, hiring, process optimization. Distributed team coordination.

### 2. Startup DNA
- **Co-founded Pegg** — Built a product from scratch, shipped to iOS/Android. Node backend, AWS/CloudFront deployment, CI/CD. Firebase real-time systems.
- **Co-founded Mirror Astrology** — Recent startup experience. Full-stack product development, LLM integration, roadmap ownership.
- **Fractional CTO work** — Shows you can context-switch, prioritize, and drive strategy for early-stage companies.
- Frame this as: "I've been on both sides — I know what it's like to build from zero AND what it takes to scale."

### 3. Technical Stack Alignment
- **TypeScript/Node.js:** Direct experience (Pegg Node backend, Scan MCP in TypeScript/Node, BHT work). List it prominently.
- **React:** Experience with React ecosystem (Kantata upgraded React). Front-end development.
- **AWS:** Production experience (Pegg deployed to AWS/CloudFront, Kantata infrastructure).
- **Kubernetes/Docker:** Deep expertise from Kantata (multiple zero-downtime K8s migrations) and Tobiko (GKE).
- **CI/CD:** CircleCI, GitHub Actions, continuous deployment — extensive experience.
- **Distributed systems/microservices:** Core strength from Kantata platform work.

### 4. Domain-Adjacent Experience
- **Integration platform (M-Bridge at Kantata):** An agent-based integration platform with databases, caching, real-time processing — architecturally similar to payment routing and checkout flows.
- **Subscription/SaaS at scale:** Kantata was a SaaS platform. You understand recurring revenue business models.
- **Real-time systems:** Firebase real-time notifications (Pegg), incident response platforms (Tobiko).

### 5. Leadership Style That Fits Their Culture
- "Clear, calm, and constructive environment" — you create focus, not chaos.
- Elevated a junior engineer to Engineering Manager (Wesley Morlock) — proof of mentorship impact.
- "No fluff" culture maps to your pragmatic, hands-on approach.
- Your recommendations speak to being deeply technical while lifting others.

---

## Growth Areas (If They Press)

Frame these honestly but positively. The recruiter likely won't dig deep here, but be prepared:

### Payments/Commerce Domain
- **What to say:** "My direct payments infrastructure experience is limited, but I've built integration platforms that handle similar patterns — routing, reliability, multi-provider orchestration, zero-downtime migrations. The M-Bridge platform at Kantata had many of the same architectural challenges as payment processing: high reliability requirements, multiple external integrations, real-time processing, and the need for 100x error reduction. I'm excited to go deep in the payments domain."
- **Don't oversell:** Don't claim payments expertise you don't have. The CTO (Stas) has deep fintech background and will see through it.

### NestJS Specifically
- **What to say:** "I haven't used NestJS specifically, but I have strong Node.js and TypeScript experience, and NestJS's opinionated structure (dependency injection, decorators, modules) is familiar territory from working with similar frameworks. I'd be productive quickly."

### Recent Role Continuity
- Your last few years have been a mix of startup/freelance/infrastructure. If they ask about the fragmentation:
- **What to say:** "After 6+ years building and leading teams at Kantata, I deliberately explored — infrastructure at Tobiko, co-founding Mirror, advising through Building Humane Technology. Each taught me something different. Now I'm looking for the right place to go deep again — a high-growth team where I can both lead and build. Phoenix checks every box."

### Pure Front-End React Depth
- Your React experience is real but not your deepest skill. If they probe:
- **What to say:** "I've worked across the full stack including React, and I'm confident building front-end features. My deeper strength is in the backend, infrastructure, and systems design — which I'd expect to be the core challenge for checkout and payments infrastructure."

---

## Questions to Ask (Show You've Done Your Research)

### About the Role & Team
1. "Which product domain would this pod own — checkout, payments, subscriptions, or dashboards? Or is that still being shaped?"
2. "How large is the pod I'd be leading, and what's the current team composition (seniority levels)?"
3. "What does 'day to day coding' look like for the Engineering Lead? What's the rough split between IC work and leadership?"
4. "What does the engineering org look like today — how many pods, and how do they coordinate?"

### About the Product & Technical Challenges
5. "You support 10+ payment processors with smart routing — what's the biggest technical challenge in that orchestration layer right now?"
6. "With 35% month-over-month growth, where is the system feeling the most strain? What would you want a new Engineering Lead to tackle first?"
7. "How are you thinking about the architecture as you scale from $350M to $1B+ GMV?"

### About Culture & Process
8. "The 'no fluff, no corporate layers' culture resonates with me. What does the engineering process actually look like day-to-day? Standups, planning cadence, deploy frequency?"
9. "How does the team balance velocity with reliability — especially for payments where downtime has real financial impact?"

### Showing Interest (Close Strong)
10. "I'm excited about this. What does the rest of the interview process look like, and what's the timeline?"

---

## Key Talking Points to Weave In

- **"I've done exactly this before"** — Built and led a team from scratch at Kantata, stayed hands-on, owned a product domain (M-Bridge, Operations platform). That's the job description.
- **"I thrive in high-growth, high-velocity environments"** — Pegg, Tobiko, Mirror were all small/fast. Kantata started as Mavenlink (startup that scaled).
- **"I care about developer experience and team health"** — Your mentorship track record (Wesley's growth from junior to EM), your coaching reputation, your DevOps culture transformation.
- **"I'm drawn to hard infrastructure problems"** — Payment routing, checkout reliability, subscription management — these are systems problems at scale. That's what energizes you.
- **"I want to go deep again"** — After exploring, you're ready to commit to a team and a domain. Phoenix's stage and pace are exactly right.

---

## Salary/Comp Notes

- Phoenix is a Series A-ish stage ($5M raise, ~30-40 people, $10M ARR).
- Remote engineering lead roles at this stage typically range $180-250K+ base depending on equity component.
- If asked, you can deflect: "I'm flexible on structure — what matters most to me is the role, the team, and the trajectory. What range does the role target?"
- Or give a range if pressed. Research suggests Engineering Lead at a high-growth startup in this space: $200-250K+ total comp is reasonable.

---

## Red Flags to Watch For (For Your Evaluation)

- **Workload/pace expectations:** "No fluff, fast-moving" can sometimes mean unsustainable hours. Ask about on-call, work-life balance.
- **Equity details:** At this stage, equity could be meaningful or negligible. Understand the cap table basics.
- **Engineering culture maturity:** With the CTO coming from Skillshare/Step, there should be real engineering culture. But a 15-month-old company with explosive growth may have accrued tech debt.
- **"No corporate layers":** Sounds good, but also means less process. Make sure you're comfortable with the level of structure (or lack thereof).
- **Merchant risk profile:** D2C, nutraceuticals, dropshipping — some of these verticals are "high-risk" in payments terminology. Understand how they think about risk.

---

## One-Liner About Why Phoenix

*"You're building the infrastructure layer that D2C merchants need to compete — checkout, payments, subscriptions, all unified. I've spent my career building exactly those kinds of platform systems, leading teams through them, and I've done it at both startup pace and enterprise scale. I'm excited to go deep on this."*
