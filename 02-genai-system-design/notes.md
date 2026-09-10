# Phase 3 — GenAI System Design

Key area of specialization — maps directly to LangChain, LangGraph, RAG, LangFuse experience.

## Core concepts
- LLM serving, model routing, prompt management, context management, token budgeting
- RAG: embeddings, vector databases, chunking, retrieval, reranking, hybrid search, query transformation, context compression, semantic caching
- LLM evaluation, hallucination mitigation, guardrails, PII/security
- Cost optimization, latency optimization
- Multi-model architectures, open-source vs. proprietary models

## Reference architecture

```
Client -> API Gateway -> AI Application
                            |         |
                        RAG Pipeline  LLM Router
                            |         |
                        Vector DB    LLM APIs
```

## Notes
_(add condensed notes here as you review)_

## Cases in this phase
- `cases/rag-for-millions-users.md`
- `cases/enterprise-ai-assistant.md`
- `cases/llm-evaluation-platform.md`
