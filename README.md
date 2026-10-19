# Đỗ Ngọc Phi

**AI Engineer · LLM agents, RAG & evaluation**
Data Science student @ Hanoi University of Mining and Geology · AI20K Build Phase (VinUni, Cohort 4)

[![LinkedIn](https://img.shields.io/badge/LinkedIn-phido0410-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/phido0410/)
[![Email](https://img.shields.io/badge/phido3107@gmail.com-D14836?style=flat-square&logo=gmail&logoColor=white)](mailto:phido3107@gmail.com)
[![GitHub](https://img.shields.io/badge/phido0410-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/phido0410)

## About me

I build **LLM applications that can be trusted in production**: the model proposes and explains, deterministic services compute the numbers, and independent validators decide what is allowed.

- Focus: LLM agents, RAG, multi-agent systems, evaluation and guardrails
- Background: machine learning, time-series forecasting and computer vision · Python

## Featured projects

### [FactoryFlow](https://youtu.be/FMUoExqVCjs) — AI agent for production order orchestration *(team of 4 · Demo Day, Oct 2026)*
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

## AI20K labs

27 daily labs in an intensive AI engineering program at VinUni, each with tests, a rubric and evidence-based grading.

<details>
<summary><b>See labs by area</b></summary>

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

</details>
