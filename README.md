<div align="center">

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=26&duration=3500&pause=800&center=true&vCenter=true&width=640&height=60&lines=Hi%2C+I'm+%C4%90%E1%BB%97+Ng%E1%BB%8Dc+Phi+%F0%9F%91%8B;AI+Engineer+%C2%B7+LLM+%26+Agentic+Systems;RAG+%C2%B7+Multi-Agent+%C2%B7+LLM+Evaluation" alt="Typing SVG" />

**Data Science student @ Hanoi University of Mining and Geology · AI20K Build Phase (Cohort 4)**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-phido0410-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/phido0410/)
[![Email](https://img.shields.io/badge/phido3107@gmail.com-D14836?style=flat-square&logo=gmail&logoColor=white)](mailto:phido3107@gmail.com)
[![GitHub](https://img.shields.io/badge/phido0410-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/phido0410)

</div>

---

## About me

I build **LLM applications that can be trusted in production** — systems where the model proposes and explains, deterministic services compute the numbers, and independent validators decide what is allowed.

- Focus: **LLM agents, RAG, multi-agent systems, LLM evaluation & guardrails**
- Recently: core engineer on **FactoryFlow**, an AI agent for production order orchestration in cement plants (AI20K Demo Day, Oct 2026)
- Background: machine learning, **time-series forecasting** and computer vision
- Main language: **Python**

---

## Featured projects

### [FactoryFlow](https://youtu.be/FMUoExqVCjs) — AI agent for production order orchestration *(team of 4 · Demo Day, Oct 2026)*
[![FactoryFlow demo video](https://img.youtube.com/vi/FMUoExqVCjs/hqdefault.jpg)](https://youtu.be/FMUoExqVCjs)

AI agent that orchestrates production orders for a 6-stage cement plant, grounded in a field study of a real plant (347 of 361 assets from anonymized plant data). **The agent proposes, CP-SAT computes, a 10-constraint validator checks, and a human approves every write.**
- Dispatcher and proactive monitor agents in a LangGraph flow with human-in-the-loop approval; rule fallback keeps it running with AI off (plan in ≤111 ms).
- CP-SAT scheduler (OR-Tools) re-plans shifts against 3 objectives: on time, keep the kiln running, fewest changes.
- Evaluated with real LLMs: 5/5 faults detected in 5–15 min with 0 false alarms, 41/41 dispatcher cases, 84/84 recovery-planner runs; 3,482 automated tests.

[Demo video](https://youtu.be/FMUoExqVCjs) · [Live demo](https://c4-app-p-022.vercel.app) · Source code is private (program repository), available on request.

`Python` `FastAPI` `LangGraph` `LangChain` `OpenAI` `OR-Tools` `PostgreSQL` `React` `TypeScript`

### [VN30 Foundation-Model Forecasting](https://github.com/phido0410/fm-finance-forecasting) — research *(team)*
Benchmark of **TimesFM, Chronos-2, Moirai-2** vs. ARIMA/LSTM for 1-day-ahead returns on Vietnamese stocks, plus **LEAF**, a lightweight regime-aware router over frozen foundation models — the only model with positive IC on the 2024–2025 test set.
- My part: LSTM baseline, VN30 data collection, zero-shot TimesFM & Chronos-2 experiments.

`PyTorch` `TimesFM` `Chronos-2` `Moirai-2` `pandas`

---

## AI20K — hands-on labs (VinUni, Cohort 4)

Intensive AI engineering program: one lab per day, each with tests, rubric and evidence-based grading.

| Area | What I built | Labs |
|---|---|---|
| **LLM & tool calling** | LLM API apps, chatbot vs. **ReAct agent** with MCP tools, tool-schema & system-prompt tuning measured on real runs | [D01](https://github.com/phido0410/K4-L3-Day1-AI-LLM-Foundation) · [D03](https://github.com/phido0410/K4A-Day03-DoNgocPhi-2A202602531) · [D04](https://github.com/phido0410/K4-DAY04-2A202602531) |
| **RAG** | Chunking & vector store → **hybrid retrieval** (dense + BM25 + RRF) with citations → **production RAG** (Qdrant, reranking, enrichment, RAGAS) → **GraphRAG** vs. flat RAG | [D07](https://github.com/phido0410/K4-L3A-DoNgocPhi-2A202602531) · [D08](https://github.com/phido0410/K4-L3A-RAG-Pipeline) · [D18](https://github.com/phido0410/K4-Track3A-DAY18-DoNgocPhi-2A202602531-ProductionRAG) · [D19](https://github.com/phido0410/K4-DAY19-DoNgocPhi-2A202602531) |
| **Agents & multi-agent** | Multi-agent system over **MCP + A2A**, agent **memory** (short-term / persistent / compaction), **Deep Agents** with subagents & self-evolving skills, **deep-research** multi-agent in a Daytona sandbox | [MCP-A2A](https://github.com/phido0410/K4-L3A-MultiAgent-MCP-A2A) · [D17](https://github.com/phido0410/K4-DAY17-DoNgocPhi-2A202602531) · [D20](https://github.com/phido0410/K4-DAY20-MULTIAGENTS-DoNgocPhi-2A202602531) · [D23](https://github.com/phido0410/K4-Day23-DoNgocPhi-2A202602531) |
| **Safety & guardrails** | Input/output guardrails, **human-in-the-loop**, red-teaming; middleware layers against hallucination, misattribution, **prompt injection** and tool-budget abuse | [D11](https://github.com/phido0410/K4-L3-DAY11-DoNgocPhi-2A202602531-Guardrails-HITL-Responsible-AI) · [D16](https://github.com/phido0410/K4-DAY16-Track3A-DoNgocPhi-2A202602531-AgentArena) |
| **Reliability & HITL** | Retry-storm game day with circuit breaker, caching, idempotency and error budget; **MCP tools** integration; **HITL PR-review agent in LangGraph** with confidence-based escalation and a replayable audit trail | [D25](https://github.com/phido0410/Track3-Day25-2A202602531-DoNgocPhi) · [D26](https://github.com/phido0410/K4-DAY26-DoNgocPhi-2A202602531) · [D27](https://github.com/phido0410/K4-DAY27-DoNgocPhi-2A202602531) |
| **Evaluation** | Golden dataset + evaluation engine scoring a real RAG system; A/B retrieval comparison (D08) and LLM-judge preference eval (D22) | [D14](https://github.com/phido0410/K4-L3A-DAY14-DoNgocPhi-2A202602531-AIEvaluation) |
| **LLMOps & deployment** | Data pipeline & observability for RAG, **Langfuse** tracing, P50/P95/P99 latency, SLO & alerts, deploying a FastAPI agent to a public endpoint with security, cost limits and zero-downtime releases | [D10](https://github.com/phido0410/K4-L3-DAY10-3ae-DataPipeline) · [D12](https://github.com/phido0410/K4-L3A-DAY12-DoNgocPhi-2A202602531-CloudServicesAndDeployment) · [D13](https://github.com/phido0410/K4-L3-DAY13-DoNgocPhi-2A202602531-Monitoring-LLMOps) |
| **Fine-tuning & alignment** | **LoRA / QLoRA** fine-tuning benchmarked against a well-prompted base model; **SFT → DPO / ORPO** preference alignment | [D21](https://github.com/phido0410/K4-Day21-DONGOCPHI-2A202602531) · [D22](https://github.com/phido0410/K4-L3-Track3-Day22-DoNgocPhi-2A202602531) |
| **AI product** | Problem framing (rule vs. workflow vs. agent); **team lead** of a two-day hackathon building a Discord assistant prototype | [D02](https://github.com/phido0410/K4A_Day02_DoNgocPhi_2A202602531) · [Hackathon](https://github.com/phido0410/K4-3A-E403-4ae) |

---

## Tech stack

**LLM & Agents**
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white)
![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=flat-square&logo=openai&logoColor=white)
![Anthropic](https://img.shields.io/badge/Anthropic-191919?style=flat-square&logo=anthropic&logoColor=white)
![MCP](https://img.shields.io/badge/MCP-000000?style=flat-square&logo=modelcontextprotocol&logoColor=white)
![Hugging Face](https://img.shields.io/badge/Hugging%20Face-FFD21E?style=flat-square&logo=huggingface&logoColor=black)

**RAG, Eval & Observability**
![Qdrant](https://img.shields.io/badge/Qdrant-DC244C?style=flat-square&logo=qdrant&logoColor=white)
![ChromaDB](https://img.shields.io/badge/ChromaDB-FF6446?style=flat-square)
![RAGAS](https://img.shields.io/badge/RAGAS-4B32C3?style=flat-square)
![Langfuse](https://img.shields.io/badge/Langfuse-0A0A0A?style=flat-square)

**ML & Optimization**
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white)
![OR-Tools](https://img.shields.io/badge/OR--Tools%20CP--SAT-4285F4?style=flat-square&logo=google&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=flat-square&logo=opencv&logoColor=white)
![pandas](https://img.shields.io/badge/pandas-150458?style=flat-square&logo=pandas&logoColor=white)

**Backend & Tools**
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Pydantic](https://img.shields.io/badge/Pydantic-E92063?style=flat-square&logo=pydantic&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)

---

<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/phido0410/phido0410/output/github-snake-dark.svg" />
  <img alt="Contribution snake" src="https://raw.githubusercontent.com/phido0410/phido0410/output/github-snake.svg" />
</picture>

</div>
