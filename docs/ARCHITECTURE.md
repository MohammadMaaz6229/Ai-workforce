# Architecture â€” AI Workforce

## Product 1: AI Support Employee

### v0.1 â€” RAG Pipeline (Phase 1)

```
Company Documents
       â†“
Document ingestion
       â†“
Chunking
       â†“
Embeddings
       â†“
Vector Database (pgvector)
       â†“
Retriever
       â†“
LLM
       â†“
Grounded Answer
       â†“
Sources / Citations
```

### v1.0 â€” Agentic Support Employee (Phase 2 target)

```
User
 â†“
AI Support Agent
 â†“
LangGraph Orchestrator
 â”œâ”€â”€ Knowledge/RAG Tool
 â”œâ”€â”€ Customer Tool
 â”œâ”€â”€ Ticket Tool
 â”œâ”€â”€ Email Tool
 â””â”€â”€ Human Escalation
```

## Design Principles

- Every AI feature follows: Input â†’ Retrieval/Context â†’ Reasoning â†’ Tool execution â†’ Validation â†’ Output.
- No unbounded LLM calls without grounding, retries, or human fallback for high-risk actions.
- Every agent action is logged and auditable.
- Prefer boring, production-proven tech over trendy tooling.

## Build Phases

1. **Foundation** â€” repo, FastAPI, DB, RAG pipeline, Docker, docs
2. **AI Support Employee** â€” LangGraph agent, tools, memory, escalation, evaluation
3. **Product** â€” auth, multi-tenancy, dashboard, billing
4. **Business** â€” deploy, demo, first customers, retention
