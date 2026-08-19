# AI Workforce

Enterprise-grade platform for deploying AI agents that perform real business workflows â€” grounded in company knowledge (RAG), capable of tool use, and safe enough for production (audit logs, human escalation, evaluation).

## First Product: AI Support Employee v0.1

An AI support agent that answers customer/employee questions using Retrieval-Augmented Generation (RAG) over company documents, with cited sources â€” and evolves toward a tool-using agent that can create tickets, send emails, and escalate to humans.

## Status

ðŸš§ Phase 1 â€” Foundation (in progress)

## Tech Stack

- **Backend:** Python, FastAPI
- **Database:** PostgreSQL + pgvector
- **Orchestration:** LangGraph
- **Frontend:** React/Next.js (added when needed)
- **Infra:** Docker, GitHub Actions
- **Testing:** pytest

## Project Structure

```
ai-workforce/
â”œâ”€â”€ app/                # Application source code
â”œâ”€â”€ tests/              # Test suite
â”œâ”€â”€ docs/               # Architecture & design docs
â”œâ”€â”€ .env.example        # Template for required environment variables
â”œâ”€â”€ .gitignore
â”œâ”€â”€ LICENSE
â””â”€â”€ README.md
```

## Getting Started

Setup instructions will be added in Step 3 (Python environment) and Step 5 (FastAPI foundation).

## Roadmap

See `docs/ARCHITECTURE.md` for the current system design and build phases.
