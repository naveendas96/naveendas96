# Hi, I'm Naveen Kumar Sivaraj 👋

**Principal Presales Solution Architect · Data, AI & Cloud · 16 years designing enterprise data platforms, now GenAI and agentic systems.**

[![Website](https://img.shields.io/badge/Navasoft-thenavasoft.com-0F766E?style=flat-square)](https://thenavasoft.com)
[![Projects](https://img.shields.io/badge/Live%20demos-thenavasoft.com%2Fprojects-FF6F61?style=flat-square)](https://thenavasoft.com/projects)
![Claude Certified Architect](https://img.shields.io/badge/Claude-Certified%20Architect-D97757?style=flat-square)
![Snowflake](https://img.shields.io/badge/Snowflake-badges-29B5E8?style=flat-square&logo=snowflake&logoColor=white)
![Databricks](https://img.shields.io/badge/Databricks-badges-FF3621?style=flat-square&logo=databricks&logoColor=white)
![Python](https://img.shields.io/badge/Python-3.11+-3776AB?style=flat-square&logo=python&logoColor=white)

## What I build

I design GenAI the way an enterprise has to run it: **grounded, permissioned, measured and costed.** Every project below ships with an architecture diagram, decision records (ADRs), a cost note, real benchmark numbers and a short demo video. All of them run at **$0** on a built-in mock model, so you can clone and verify in minutes with no API key, then switch to Ollama, OpenAI or Anthropic with one environment variable.

- 🔎 **Retrieval you can audit:** hybrid search, access control before retrieval, cited answers, refusal when the documents don't know
- 🤖 **Agents with guardrails:** typed state machines, bounded loops, deterministic numbers, human review where it matters
- 🧮 **Data platforms × AI:** semantic layers, safe SQL, Snowflake / Databricks / DuckDB adapters
- 🔌 **Tooling for AI assistants:** governed MCP servers with scopes and audit trails
- 📏 **Evals as a release gate:** quality, safety, latency and cost compared run over run, CI fails on regression

## Featured projects

| Project | What it proves | Real results (mock-model run, reproducible with `make`) |
|---|---|---|
| [**enterprise-rag-reference**](https://github.com/naveendas96/enterprise-rag-reference) | Enterprise RAG with RBAC, citations and grounded refusal | hit@4 **1.00** · refusal accuracy **1.00** · RBAC leaks **0** · citation correct **0.92** · answer correct **0.85** (17-case golden set, 4 roles) |
| [**presales-copilot-agents**](https://github.com/naveendas96/presales-copilot-agents) | Four LangGraph agents turn an RFP into a traceable draft proposal | **12/12** requirements extracted · **10/10** must-haves covered · **296.2** person-days estimated · **12** risks · under 1 s |
| [**lakehouse-text2sql-agent**](https://github.com/naveendas96/lakehouse-text2sql-agent) | Governed text-to-SQL over a lakehouse star schema | execution accuracy **0.79** (11/14) · guardrail block rate **1.00** (8/8 attacks) · misses documented on purpose |
| [**enterprise-mcp-toolkit**](https://github.com/naveendas96/enterprise-mcp-toolkit) | Three governed MCP servers (ITSM, data, docs) for Claude Desktop / Cursor | **15/15** tests: hidden write tools, scope denial, 5 SQL attack patterns, docs ACL, secret redaction in the audit log |
| [**agent-eval-harness**](https://github.com/naveendas96/agent-eval-harness) | Eval + regression gating + dashboard for LLM agents | Blocked a "cheaper prompt" that was **29% cheaper and 33% faster** but dropped safety **1.0 → 0.778** and groundedness **1.0 → 0.5** |

▶️ Short demo videos of each run: **[thenavasoft.com/projects](https://thenavasoft.com/projects)**

<details>
<summary><b>How I work (the pattern behind all five repos)</b></summary>

1. **Local-first and pluggable:** `LLM_PROVIDER=mock|ollama|openai|anthropic`. CI is deterministic and free.
2. **LLMs for language, code for numbers:** estimates, metrics and SQL limits are deterministic and explainable.
3. **Governance at the boundary:** permissions are checked before retrieval and before tool calls, not after generation.
4. **Every loop is bounded:** critic loops, self-correction and retries have hard caps, so cost can't run away.
5. **Evals gate releases:** a change that's cheaper but less safe doesn't ship.
</details>

## Work with Navasoft

I run **[Navasoft](https://thenavasoft.com)**, a small studio for GenAI and agentic AI architecture.

- **RAG / Agent PoC in 2 weeks:** a fixed-scope prototype on your own data, with an eval report and a go / no-go recommendation
- **Architecture reviews:** pressure-test your RAG, agent or text-to-SQL design for retrieval quality, evals, cost and security
- **Enterprise GenAI Starter Kit:** the setup guide, architecture and ADR templates and eval checklist I use on these projects

👉 **[thenavasoft.com](https://thenavasoft.com)**: start a conversation there.

<!-- Uncomment after GitHub Sponsors is approved:
💚 If these repos save you time, [sponsor the work](https://github.com/sponsors/naveendas96).
-->

<sub>Numbers come from each repo's own `make eval` / `make bench` / `make demo` run on the deterministic mock model; re-verified 19 Oct 2026. Real-model numbers will differ, and each README explains how to measure them.</sub>
