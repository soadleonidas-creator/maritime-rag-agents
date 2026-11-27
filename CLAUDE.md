# CLAUDE.md

## Project
Multi-agent RAG assistant over public maritime documents. Portfolio flagship: production-grade, reliable, cost-aware.

## Rules
- Public or synthetic data only. Never add employer data, documents, code or credentials.
- Never commit secrets. API keys come from environment variables (`.env` is gitignored).
- Plan before coding. Record significant tool choices as a decision record in `docs/decisions/`.
- Each agent tool goes through an MCP server in `services/`, not direct function calls.
- Every behavior change needs an eval case in `evals/`.
- Track cost: every LLM call records model, tokens and cost in its trace.
