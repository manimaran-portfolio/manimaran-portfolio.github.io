# Manimaran Gandhikumar

### GenAI Architect & Test Lead | Multi-Agent Systems · RAG · Applied LLM Engineering

📍 Mississauga, Ontario, Canada
🔗 [Portfolio](https://manimaran-portfolio.github.io/) · [LinkedIn](https://www.linkedin.com/in/manimaran-g2707/) · [Credly Badges](https://www.credly.com/users/manimaran-gandhikumar.50614893)
✉️ manimaran990@gmail.com

---

## 👋 About Me

Applied AI Architect and GenAI Test Lead with **10 years in Capital Markets and Banking**, building at the intersection of **agentic AI, data engineering, and quality automation**.

At Cognizant (RBC Capital Markets), I architect **self-evolving multi-agent systems** — an AI Agent Factory, Meta Agent routing layer, and custom RAG pipelines — that transform traditional testing lifecycles into autonomous, AI-driven operations, all while meeting stringent financial data governance on real-time (Kafka) and batch (PySpark) platforms.

I'm also a hands-on **self-hosted AI homelabber**: Docker-based local LLM inference (Ollama, Hermes), agent orchestration frameworks, and privacy-first AI tooling.

---

## 🏆 Certifications

**Anthropic — Claude Foundations (2026)**

- **Claude Certified Architect – Foundations** — Issued Aug 2026 · production-grade design with Claude Code, Agent SDK, API & MCP
- **Claude Certified Associate – Foundations** — Issued Aug 2026 · business applications, output evaluation & responsible use
- **Claude Certified Developer – Foundations** — Issued Sep 2026 · building & shipping production apps and agents with Claude API, Claude Code, custom tools & MCP

Full badge wallet: [Credly Profile](https://www.credly.com/users/manimaran-gandhikumar.50614893)

**Other certifications:** Python for Data Science and AI · Introduction to Data Engineering · Linux Commands & Shell Scripting · ETL and Data Pipelines (Airflow/Kafka) · Python Project for Data Engineering

---

## 🛠 Technical Skills

| Domain | Skills |
|--------|--------|
| **Generative AI & Agentic Workflows** | Multi-Agent Orchestration (CrewAI, LangChain), Meta Agents (Autonomous Routing), Self-Evolving System Prompts, Semantic Memory Systems |
| **Applied AI & RAG** | Retrieval-Augmented Generation (RAG), Vector Databases, Context Window Optimization, Open-source LLMs (Ollama, LM Studio) |
| **AI-Ops & Architecture** | Local LLM Inference, Docker Self-Hosting, Backend APIs (FastAPI, Python), Dashboards (NiceGUI, Streamlit) |
| **Data & Quality Engineering** | Real-time Streaming (Kafka), Batch (PySpark/Spark), Core Java, Advanced SQL, CI/CD (Jenkins, GitHub Actions) |
| **Testing & Automation** | Selenium, Pytest, Cucumber, Regression Frameworks, FIX Protocol Testing |

---

## 💼 Experience

### Cognizant — GenAI Developer & Test Architect (RBC Capital Markets)
*Apr 2024 – Present · Toronto, ON*

- Architected an **AI Agent Factory** and **Skill Factory** to automate complex development and testing lifecycles, accelerating time-to-market
- Engineered **self-evolving autonomous agents** with stateful memory — nightly prompt evaluations drive continuous accuracy optimization
- Designed a **node-based Visual Workflow Builder** and Chat UI for seamless agent-to-agent communication and user-driven automations
- Built a **Meta Agent routing layer** that parses requests, delegates to specialized sub-agents, and consolidates responses
- Developed a custom **RAG pipeline** over proprietary project documentation, drastically reducing onboarding time
- Embedded automated **data-quality verification gates** into real-time Kafka streams and PySpark batch pipelines for trade and risk datasets

### Infosys — Python Developer / QA (Morgan Stanley, Exchange Connectivity)
*Oct 2019 – Apr 2024 · Montreal, QC*

- Engineered an **Exchange Connectivity Dashboard** (FastAPI/Flask backend, SPA frontend) to control exchange instances, send FIX messages, and manage jobs from a single place
- Built regression and **FIX message replay** frameworks, delivering ~40% performance improvement in testing efficiency
- Led the **Xray/Jira integration service** — a FastAPI test-manager service automating test execution and Jira sanity for multiple internal teams

### Infosys — Python Developer (Morgan Stanley, Offshore)
*Sep 2018 – Oct 2019 · India*

- Python ETL validation, schema checking, and dataset reconciliation; automated pipelines via Jenkins with pytest coverage
- Piloted PySpark jobs to verify transformation logic for downstream risk analytics

### Infosys — Technology Engineer (Citi, Payments & Digitization)
*Dec 2015 – Sep 2018 · Chennai, India*

- Built an **Ingestion Testing framework** (Kafka/HBase) cutting test reporting from 40 minutes to 2 minutes; validates 1M+ records with 300+ columns in under 3 minutes
- Developed a **Payment Tracker** utility tracing high-speed transactions across Kafka, HBase, and Ignite for compliance and environment readiness

---

## 🤖 Agentic AI Portfolio Projects

Five production-pattern agent systems showcasing the 2025/26 industry stack — MCP, human-in-the-loop, multi-agent supervision, GraphRAG, hybrid local/cloud inference, evals & observability. Each runs with a single `docker compose up`, is demoable live in 5–8 minutes, and streams traces to a Langfuse/Phoenix dashboard.

### 1. TradeBreak Copilot — Settlement Break Resolution Agent
Autonomous agent that reconciles broken trades across multi-broker FIX feeds, diagnoses root causes, and generates auditable repair tickets — with a hard human-approval gate above $10K exposure.
**Stack:** LangGraph (HITL interrupt states) · MCP server exposing FIX simulator + mock OMS + DuckDB · Claude (reasoning) + local Ollama (PII redaction) · NeMo Guardrails + DeepEval · Langfuse tracing · Streamlit diff viewer.
**Demo flow:** inject 20-trade batch with 3 breaks → agent detects break signatures via MCP tools → proposes correction with confidence score → **HITL pause** on >$10K break → approve → show ledger update + full Langfuse trace.
*Demonstrates: MCP tool design, HITL/checkpointed state graphs, legacy financial infra integration, audit compliance.*

### 2. ChaosAgent — Automated LLM Red-Teaming Harness
Multi-agent adversarial swarm that jailbreak-stress-tests LLM applications, scores vulnerabilities against the OWASP GenAI Top 10, and auto-generates pytest regression suites from every failure.
**Stack:** LangGraph swarm (Attacker / Target-proxy / Judge agents) · PyRIT + Giskard + pytest · PostgreSQL attack-vector lineage · Arize Phoenix tracing · HTML report generator.
**Demo flow:** point Attacker at a mock financial assistant → multi-turn jailbreak evolves (obfuscation → Base64 → recursive framing) → Judge flags LLM01/LLM06 → one command emits a failing pytest case wired into CI.
*Demonstrates: automated red-teaming, continuous eval pipelines, QA-to-LLMOps depth — perfect for a Test Architect profile.*

### 3. SentinelStream — Real-Time Market Surveillance Agents
Streaming multi-agent surveillance engine that triages high-throughput trader chatter locally and escalates only anomalies to a frontier cloud agent for investigation.
**Stack:** Kafka (100 msg/s simulated Bloomberg chats) · local vLLM 7B triage filter (~35ms, 95% of benign traffic, $0 API cost) · Claude escalation agent · Redis sliding context + LanceDB precedent search · Prometheus/Grafana · WebSocket alert dashboard.
**Demo flow:** stream routine chatter (95% filtered locally) → inject collusion + abnormal options volume → escalation agent drafts an SEC TCR-compliant narrative with timestamps → Grafana shows cost/latency/edge-offload metrics.
*Demonstrates: hybrid local/cloud LLM tiering, latency-critical streaming, cost engineering, regulatory domain fluency.*

### 4. ForensicRAG — Graph-Native Financial Document Intelligence
GraphRAG system that parses multi-year 10-Ks and earnings calls into a Neo4j knowledge graph to expose cross-filing contradictions — with citations down to the PDF bounding box.
**Stack:** Neo4j + LlamaIndex PropertyGraphIndex · Docling (structure-preserving table parsing) · Claude + text-embedding-3-large · Ragas + TruLens faithfulness evals · Streamlit graph explorer with PDF deep-links.
**Demo flow:** ingest two 10-Ks + earnings transcript → ask "compare executive debt-maturity claims vs. footnote commitments" → multi-hop traversal surfaces a $45M contradiction, cites exact nodes and highlights the source PDF region → Ragas report shows Faithfulness = 1.0.
*Demonstrates: why vector-only RAG fails on tabular financial data, GraphRAG multi-hop reasoning, grounded citations, hallucination evals.*

### 5. RiskTwin — Multi-Agent Market Stress-Testing Simulator
Hierarchical persona-driven agent swarm (Market Maker, Hedge Fund, Retail Sentiment) simulates systemic shocks and cascading liquidity effects on a live portfolio, ending in an executive risk memo.
**Stack:** LangGraph supervisor + shared blackboard memory · NumPy/SciPy/Riskfolio-Lib (VaR, expected shortfall, market impact) · Claude reasoning · Plotly reactive dashboards.
**Demo flow:** seed a $500M portfolio + "50bps surprise rate hike + regional bank credit freeze" → agents react step-by-step (spread widening, stop-loss liquidations, panic redemptions) → charts show VaR spiking live → Supervisor compiles a Risk Committee Memo with contagion paths and hedge recommendations.
*Demonstrates: hierarchical multi-agent supervision, shared-state blackboard architecture, LLM + quantitative modeling fusion.*

**Common build standards across all five:** typed Pydantic schemas everywhere (no prompt salad) · Langfuse/Phoenix tracing with token & latency telemetry · `DEMO_MODE=deterministic|live` toggle so no live demo can flake · hybrid local/cloud LLM routing with local Ollama/vLLM fallback · single-command `docker compose up` bootstrap · 90-second demo GIF in each README.

---

## 🚀 Independent & Product Projects

### TradesPulse
AI-powered missed-call and lead-tracking platform for trades businesses — converting missed calls into actionable leads with automated follow-up.
*Status: in active development (private repo)*

### Mississauga Lead Feed
Automated local lead-scraping and delivery pipeline for Mississauga/Toronto — scheduled scraping, enrichment, and notification workflows.
*Status: in active development (private repo)*

### Self-Hosted AI Homelab
Docker-based private AI infrastructure: local LLM inference, multi-agent orchestration, self-hosted productivity and note-taking apps — built for privacy-first, air-gapped operation.

### Earlier projects
- [Expense Tracker](https://github.com/manimaran990/expenseTracker) — Django money-tracking app with spending analysis and LLM-driven suggestions
- [Second Brain](https://github.com/manimaran990/secondBrain) — ChatGPT-style note-taking app ingesting URLs, YouTube links, images and Markdown, with a Chrome plugin and Telegram bot

---

## 🎓 Education

**Master of Computer Applications (MCA)** — College of Engineering Guindy, India (2015)

---

<p align="center">
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/python/python-original.svg" alt="Python" width="40"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/fastapi/fastapi-original.svg" alt="FastAPI" width="40"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/docker/docker-original.svg" alt="Docker" width="40"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/apachekafka/apachekafka-original.svg" alt="Kafka" width="40"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/pyspark/pyspark-original.svg" alt="PySpark" width="40"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/git/git-original.svg" alt="Git" width="40"/>
</p>