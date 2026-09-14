# 👋 Siddhant Patil
**Founder @ Black Robotics 🤖 | 2x founding AI engineer | robotics + AI | MS CS @CSULB**

🤖 Founder, **Black Robotics**: data pipelines for humanoid robot training
🎯 Founding AI Engineer, **Teamcast.ai**: hiring intelligence
🎓 M.S. Computer Science, CSULB · 📍 Mountain View, CA

I build AI systems that hold up under real conditions: partial data, changing rules, and the messy seam where models meet the physical world.

💻 **[siddhantnitin.com](https://siddhantnitin.com)** has the long-form case studies.

---

## Selected Work

Every number below was measured by the eval harness committed in that project, not estimated.

### 🏥 PolicyDesk: permission-aware policy knowledge system
**FastAPI · Postgres + pgvector · Gemini · Vercel + Supabase**

Staff at a (synthetic) regional health plan ask policy questions and get answers cited to the current policy section, filtered to what their role may see. The permission filter lives inside the retrieval SQL, so restricted text never reaches ranking or the model.

- **0 of 900** unauthorized chunks reached the model (50 questions × 3 roles)
- **95.0%** correct-and-cited answers, **100%** refusal correctness on a 50-question golden set
- Retrieval and generation measured separately (recall@5 97.1%), p50 latency 2.9 s
- Version resolution, conflict detection and refusals run in code, outside the model

▶️ [Live demo](https://policydesk-nine.vercel.app) · 📄 [Case study](https://siddhantnitin.com/work/policydesk)

### 🛡️ PALADIN: account research that refuses to invent facts
**FastAPI · Postgres · Gemini · LangGraph (for one durable approval step)**

Takes a CSV of target accounts, reads each company's site, keeps only facts whose quote appears verbatim on the page, scores the account in plain code, and drafts a brief that may only cite those facts. A human approves before anything is exported to HubSpot.

- Restricting drafts to cited facts cut unsupported claims from **27.7% to 6.9%** on identical inputs (human audit)
- Research fact precision **84.4%**, recall **96.8%** against labels
- Failures documented, including the ones the code checks did not catch

🐙 [Repo](https://github.com/siddhant8019/palaadin)

### 🎙️ Maya: live AI interviewer at Teamcast
A real-time voice interviewer and the scoring system behind it, built so every automated judgment traces back to something a candidate actually said.

📄 [Case study](https://siddhantnitin.com/work/maya)

---

## What I'm Building Now

### 🤖 Black Robotics
🌐 [blackrobotics.tech](https://blackrobotics.tech)

The bottleneck for humanoid robots isn't models, it's **standardized, high-quality training data**. Teleoperation logs, sim rollouts, and demonstration data live in fragmented formats across labs and embodiments. Black Robotics is building the pipeline layer that makes this data trainable, comparable, and portable across platforms.

---

### 🎯 Teamcast.ai
**FastAPI · async Python · Pydantic v2 · SSE streaming · Postgres · GCP**

Hiring reframed as **constraint-based decision making**. I work across the stack:

- **AI assessment:** three decoupled pipelines (pre-interview scaffolds, real-time signal routing, post-interview scoring)
- **Integrations:** Apollo, Greenhouse, Deel
- **GTM engine:** 5-agent outbound system with ICP signal pipelines
- **Observability:** Arize Phoenix for eval loops and audit trails
- **Ops:** investor outreach, CAB tracking, onboarding, seed-raise support

---

## How I Think About AI Systems

- Determinism over surprise
- Evaluation before scale
- Infrastructure before prompting
- Constraints before cleverness

If a system can't explain why it acted, retry safely, or adapt when rules change, it's not production-ready.

---

## Writing

I publish on **Physical AI and robotics first** (humanoid foundation models, embodied AI, fleet deployment), with LLM and agent infrastructure as secondary scope.

Style: contrarian, benchmark-driven, systems-thinker framing. No hype, no hedging.

✍️ [medium.com/@siddhantnitin](https://medium.com/@siddhantnitin)

---

## Stack

**Languages:** Python, TypeScript, SQL
**LLMs & Agents:** RAG, permission-aware retrieval, agent orchestration, evaluation loops, LangGraph
**Backend:** FastAPI, async/await, SSE, Pydantic v2, pytest, Postgres + pgvector, Redis, Docker
**Ops:** Arize Phoenix, Vercel, Supabase, validation systems, workflow orchestration

---

## Connect

🔗 [LinkedIn](https://www.linkedin.com/in/siddhantnpatil) · 🐦 [X](https://x.com/siddhant_8019) · 💻 [siddhantnitin.com](https://siddhantnitin.com) · 🐙 [GitHub](https://github.com/siddhant8019)
