# Interview Prep — ForUsAll Senior Ruby on Rails AI Systems Engineer

**Stage**: Onsite interview (Oakland, 6520 Telegraph Ave, Unit 2)
**Interviewers**: Mike (Senior Rails Eng) + Jorge Iriso (Rails Eng)
**Format**: 45–60 min; short technical exercise (2D array, real-time discussion)
**Date**: TBD (scheduling in progress as of 2026-04-17)

---

## 1. Quick Company Brief

**What they do**: ForUsAll is a 401(k) platform for startups and small businesses — modern retirement benefits with crypto access built in. Founded 2013, Series B, $49.5M raised. ~40 people, split Oakland (eng leadership + 2 senior Rails engineers) and Medellín (2 AI engineers, 1 DevOps).

**Tech stack**: Ruby on Rails, StimulusJS/Hotwire, PostgreSQL, Sidekiq, modern LLM APIs

**Engineering today**: Small team in Oakland. They're actively incorporating AI agents at every layer — UI, backend, code management, and potentially the product itself. Hiring 2 in SF + 2 more in Medellín.

**CTO**: Bhavani Yanamadala (your round 2 virtual). Title on company site is CTO; Trista called her "head of engineering."

**Glassdoor signal**: 2.1/5 overall, 22% recommend. Reviews cite toxic management culture, previous Head of Engineering firing, high turnover. Treat this as a live evaluation during the onsite — probe directly with Mike and Jorge.

---

## 2. Key People

### Jorge Iriso — Rails Engineer (onsite interviewer)
- Background spans fintech/security: IBM, Charles Schwab, Wells Fargo, Proofpoint, Nexgate
- AI Consultant at Tedigo.net before ForUsAll
- Full Stack at boxBot (2019–2021)
- Education: BS Universidad Politécnica de Madrid, MS Syracuse
- **What this tells you**: He's been around the block — not a junior. Likely values pragmatic engineering over hype. His AI consulting background means he'll respect real-world LLM experience over buzzwords.

### Mike — Senior Rails Engineer (onsite interviewer)
- Last name unknown. Senior title suggests more tenure than Jorge.
- **Approach**: Ask him what he's been working on. Peer engineers are usually candid if you're genuinely curious.

### Bhavani Yanamadala — CTO (round 2)
- Listed as CTO on forusall.com/about
- Previous Head of Engineering was apparently let go (Glassdoor signal)
- **What to ask**: How long she's been in the role, how the team has evolved, what the eng roadmap looks like for the next 6 months.

---

## 3. What to Expect at the Onsite

**Technical exercise**: 2D array problem. Real-time problem-solving discussion. No prep required per Trista. But know your fundamentals cold:
- Matrix traversal (BFS/DFS, row/column iteration)
- Common patterns: rotating a matrix, spiral traversal, island counting, diagonal traversal
- In Ruby, just use nested arrays: `matrix[row][col]`
- Think out loud. They want to see your reasoning process, not just the answer.

**Interview dynamic**: They reached out to you (inbound). That's leverage. You're evaluating them as much as they're evaluating you.

**What they're optimizing for**: Someone who can teach them about AI/LLMs. Lead with concrete production examples. They may not have precise language for what they want — your job is to define the conversation.

---

## 4. What to Lean Into

### Crown Jewel: AI in Production
- Mirror Astrology: built a production Rails app with a multi-LLM chatbot (tool use, context augmentation, streaming). Real paying users. You built the whole stack.
- BHT/HumaneBench: eval framework for measuring LLM behavior in production workflows. Python, but shows AI engineering depth.
- Key talking point: "I've shipped AI features in production Rails apps and built the eval infrastructure to measure whether they're actually working."

### Rails Depth
- Rails practitioner since 2008 — longer than ForUsAll has existed.
- Kantata: led migration of the entire Rails monolith and all services to Kubernetes (zero-downtime). Led Ruby/Rails upgrade strategy across the engineering org.
- M-Bridge: background job system driving multi-system integrations at scale — reduced errors ~100x.
- Key talking point: "I know the full Rails lifecycle — not just building features, but upgrading the platform, migrating infrastructure, and keeping background job systems reliable at scale."

### Agentic Workflows
- Their job description specifically calls out "incorporating agents at every layer" and "building agentic workflows." This is your strongest differentiator.
- Talk about MCP, tool use, multi-agent patterns. HumaneBench eval work shows you think rigorously about AI behavior.
- Key talking point: "I've been building with agent frameworks and LLM tool use since before it was mainstream — eval discipline is part of the workflow, not an afterthought."

### Small Team, Big Ownership
- Kantata: built and rebuilt teams from near-zero (DevOps team rebuild after mass departures).
- Mirror: owned the entire stack as a co-founder.
- At ForUsAll's team size, your ownership instinct is a strength, not overhead.

---

## 5. Growth Areas — Be Honest

**Fintech / 401(k) domain**
- You don't have 401(k)-specific domain experience. That's fine — it's compliance and financial data, not radically different engineering.
- What to say: "I don't have fintech-specific domain knowledge, but I've worked in regulated engineering contexts and I ramp up on domain constraints quickly."
- Don't pretend you know 401(k) compliance rules.

**StimulusJS / Hotwire specifically**
- If pressed: "I've been building Rails apps with the modern frontend stack — Hotwire is the Rails default and I know the patterns — but my most recent work has been primarily on the backend and AI integration layers."
- Don't claim deep Hotwire expertise if you haven't shipped Hotwire-heavy features.

**Sidekiq in production at scale**
- You've led teams running background job systems at scale (M-Bridge), but may not have personally written Sidekiq workers recently.
- What to say: "I've operated background job infrastructure at scale and understand the failure modes well. Sidekiq itself I'd pick up in the first week."

---

## 6. Questions to Ask

### Role & Team
- "What are Mike and Jorge each working on right now that you're most excited about?"
- "What does the agentic workflow layer look like today, and where do you want it to be in 6 months?"
- "How does the Oakland team collaborate with the Medellín team day-to-day?"

### Technical
- "What's your approach to background job reliability and failure handling with Sidekiq?"
- "How are you thinking about evals for the AI features you're shipping — how do you know they're working?"
- "What does the deploy pipeline look like? How often are you shipping?"

### Culture / Probing the Red Flags (ask Mike and Jorge, not in round 1 with Trista)
- "What's the tenure of the engineers on the team? You two been here a while?"
- "How does the team handle postmortems — when something goes wrong, how do you figure out what happened?"
- "What's the on-call situation like?"
- "How does Bhavani work with the engineering team — is she in the weeds technically or more strategic?"

### Close Strong
- "What would make someone a clear 'yes' after seeing their take-home?"

---

## 7. Key Talking Points

1. "Rails since 2008, AI since it got real — I've been building production LLM features in Rails apps for the last two years."
2. "The M-Bridge platform I led ran ~100x more reliably after we rebuilt it — that was background jobs, monitoring, and disciplined incident response."
3. "I built the whole stack at Mirror — Rails backend, frontend, AI chatbot with tool use and context augmentation. Paying users in production."
4. "I've led teams through the hard migrations — Rails monolith to Kubernetes, zero downtime — so I know what 'reliability' costs and how to deliver it."
5. "I'm the person who brings eval discipline to AI work: not just 'does the LLM respond,' but 'is it actually doing the right thing in production?'"

---

## 8. Salary / Comp Notes

- Trista's stated range: $120–200k. Wide range = they're flexible.
- Don't anchor low. Your background anchors closer to $180–200k for a principal-level IC.
- If asked for a number in the onsite, deflect: "I'm focused on understanding the role and team — I'd want to know more before I give you a number that's fair to both of us."
- If pushed: "Based on my background and the market, I'm targeting around $180k. Is that in range for this role?"

---

## 9. Red Flags to Watch For

- **Toxic culture tell**: Do Mike and Jorge answer culture questions with deflection or corporate-speak? Ask them directly how long they've been there and whether they'd make the same choice again.
- **Scope / ownership clarity**: Is the role clearly defined, or does it sound like "do everything"? Burnout at small startups often comes from unclear scope.
- **Previous HoE**: If it comes up naturally, ask "what happened?" and watch the reaction. Blaming the engineer is a red flag; owning the transition is a green flag.
- **Comp ceiling**: $120–200k range is wide. If they anchor you toward $120k, that's a signal.
- **AI vision vs. reality gap**: Do they actually have a coherent AI architecture, or is it "we want to add AI to things"? Ask about current state, not future aspirations.

---

## 10. One-Liner

"I'm a Rails engineer who's been shipping AI features in production since before it was a job title — and I bring the eval discipline to know whether they're actually working."

---

## Sources

- [ForUsAll Glassdoor Reviews](https://www.glassdoor.com/Reviews/ForUsAll-Reviews-E1145530.htm)
- [ForUsAll Software Engineer Reviews](https://www.glassdoor.com/Reviews/ForUsAll-Software-Engineer-Reviews-EI_IE1145530.0,8_KO9,26.htm)
- [Jorge Iriso — ZoomInfo](https://www.zoominfo.com/p/Jorge-Iriso/1783939262)
- [Senior Ruby on Rails Engineer @ ForUsAll — Foundation Capital Job Board](https://jobs.foundationcapital.com/companies/forusall/jobs/54578754-senior-ruby-on-rails-engineer)
