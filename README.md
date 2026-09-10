# System Design for AI/ML

A personal study and portfolio repo for System Design applied to ML, GenAI, and Agentic systems — built to prepare for ML Engineer / AI Engineer / GenAI Engineer interviews.

**Author:** Gilson Vieira de Souza — Machine Learning Engineer (GenAI & AI Engineering)
**Companion repo:** [`language-ai-engineering-lab`](#) — conceptual/learning notebooks live there; this repo is applied design + interview prep.

---

## Why this structure

Most "system design" prep treats every topic as equally weighted. This roadmap instead follows a deliberate progression:

```
Software System Design → ML System Design → GenAI System Design → Agentic System Design
```

Each phase builds on the last, and maps directly onto real experience (Spring Boot/Kafka/Terraform → SageMaker/MLflow → LangChain/RAG → LangGraph/MCP), so studying doubles as articulating what I already do in production.

Every completed case follows the same 15-point structure (see [`_templates/design-doc-template.md`](_templates/design-doc-template.md)), so depth is comparable across topics and the format becomes second nature under interview pressure.

---

## Progress tracker

### Phase 0/1 — Fundamentals (refresher, not deep study)
- [ ] Scalability, availability, reliability, CAP theorem
- [ ] Load balancing, caching, queues, API design
- [ ] Architecture patterns: CQRS, Saga, circuit breaker, rate limiting

### Phase 2 — ML System Design
- [ ] ML lifecycle: ingestion → feature store → training → serving → monitoring
- [ ] Batch vs. online inference
- [ ] Data/concept drift, retraining, A/B & canary/shadow deployment
- **Cases:**
  - [ ] `fraud-detection.md`
  - [ ] `recommendation-system.md`
  - [ ] `ml-inference-platform.md`

### Phase 3 — GenAI System Design
- [ ] LLM serving, routing, prompt & context management, token budgeting
- [ ] RAG: embeddings, chunking, retrieval, reranking, hybrid search
- [ ] Evaluation, hallucination mitigation, guardrails, cost/latency optimization
- **Cases:**
  - [ ] `rag-for-millions-users.md`
  - [ ] `enterprise-ai-assistant.md`
  - [ ] `llm-evaluation-platform.md`

### Phase 4 — Agentic System Design
- [ ] Agent architecture, tool calling, ReAct, memory (short/long-term)
- [ ] Multi-agent orchestration, human-in-the-loop, MCP, tool registry
- [ ] Agent evaluation, tracing, failure recovery, cost/latency control
- **Cases:**
  - [ ] `multi-agent-customer-support.md`
  - [ ] `mcp-enterprise-agent-platform.md`

---

## Repo structure

```
system-design-ai/
│
├── README.md
├── 00-fundamentals/
│   └── notes.md
├── 01-ml-system-design/
│   ├── notes.md
│   └── cases/
├── 02-genai-system-design/
│   ├── notes.md
│   └── cases/
├── 03-agentic-system-design/
│   ├── notes.md
│   └── cases/
├── _templates/
│   └── design-doc-template.md
└── diagrams/
```

- **`notes.md`** per phase — condensed reference notes, not a folder-per-concept. Searchable, not sprawling.
- **`cases/`** — completed design docs. This is the portfolio: what a recruiter or interviewer would actually open.
- **`_templates/`** — one reusable design doc template, applied consistently to every case.
- **`diagrams/`** — architecture diagrams referenced by relative path from cases, centralized so formats stay consistent.

## How to use this repo

1. Pick a case from an unstarted phase.
2. Copy `_templates/design-doc-template.md` into the phase's `cases/` folder, rename it.
3. Fill it out end-to-end — no skipping sections, even weak ones. Weak sections reveal what to study next.
4. Check it off above.
