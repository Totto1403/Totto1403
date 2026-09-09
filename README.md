# Hi there, I'm Bharanee! 👋

### GenAI & Agentic Systems | Backend Engineering | Applied Machine Learning
**B.Tech Computer Science @ VIT Chennai** &nbsp;|&nbsp; **B.S. Data Science & Applications @ IIT Madras**

---

I build production-grade **Agentic AI systems**, high-concurrency **backend infrastructure**, and **applied machine learning pipelines**. Comfortable owning complex systems end-to-end — from database and retrieval architecture to low-latency deployable APIs and agent loops.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/bharanee-b-a387902b5/)
[![GitHub](https://img.shields.io/badge/GitHub-Profile-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Totto1403)
[![Email](https://img.shields.io/badge/Email-bharanee1403%40gmail.com-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:bharanee1403@gmail.com)

---

## 🚀 Featured Projects

### 🧠 [Enterprise Multi-Agent Intelligence Engine](https://github.com/Totto1403/multiagent-mcp-rag)
*Tech Stack: Python, LangGraph, FastMCP (Model Context Protocol), Qdrant, BM25, FastAPI, Pydantic v2, SQLite, Ragas*
- Architected an asynchronous multi-agent enterprise platform orchestrating Supervisor routing, self-correcting NL-to-SQL generation, and citation-grounded Hybrid RAG over financial transaction databases and credit policy documents.
- Built a two-stage retrieval pipeline fusing dense vector search (Qdrant 1536d) and sparse keyword retrieval (BM25 Okapi) via Reciprocal Rank Fusion (RRF, $k=60$) and Cross-Encoder reranking (100% Context Precision).
- Decoupled tool services via FastMCP (Stdio/SSE) with AST-level SQL validation and streamed live token/thought traces via FastAPI SSE backed by Pydantic guardrails (117ms median latency).

### ⚡ [MicroAgent: Zero-Framework Single-Agent ReAct Engine](https://github.com/Totto1403/microagent-from-scratch)
*Tech Stack: Python 3.10+, ReAct Loop, Pydantic v2, OpenAI API, Rich, Pytest*
- Built a transparent, zero-framework autonomous AI agent from scratch in pure Python to master agent internals without third-party framework abstractions.
- Engineered an AST-inspected `@tool` decorator that dynamically transforms native Python function signatures, type annotations, and docstrings into OpenAPI/JSON schemas.
- Implemented an adaptive self-healing execution loop that traps runtime exceptions (e.g. syntax errors) into diagnostic observations for automated LLM self-correction.
- Added sliding-window context pruning, token budget estimation, and Human-in-the-Loop (HITL) approval gates.

### 🚗 Driver Risk Assessment System (DRAS) — Final-Year Capstone
*Tech Stack: Python, PyTorch, OpenCV, YOLOv8, ResNet-34, Scikit-learn | Team of 3*
- Engineered an edge-deployable multimodal pipeline fusing facial-expression recognition (ResNet-34), adaptive eye-aspect-ratio fatigue detection, head-pose estimation, and YOLOv8-based phone distraction detection into a single real-time driver risk score.
- Designed a late-fusion scoring model (70:30 visual-behavioral to affective weighting) across 4 perception streams, achieving **93.17% accuracy on the NTHU-DDD benchmark** (outperforming the published 90.48% baseline).
- Built continuous baseline-calibration logic to eliminate false positives from fixed-threshold fatigue detection for real-time edge inference.

### 🏢 [Placement Portal Application](https://github.com/Totto1403/placement-portal)
*Tech Stack: Python, Flask, Vue.js 3, Redis, Celery, JWT, SQLAlchemy*
- Built a decoupled REST API with JWT-secured Role-Based Access Control (RBAC) powering distinct Admin, Company, and Student workflows across the campus recruitment lifecycle.
- Integrated Redis caching and Celery background asynchronous task queues to cut database load on high-traffic endpoints; shipped a responsive Vue.js 3 / Vite SPA with PWA support.

### 📊 Applied Machine Learning & Competitive Modeling — Kaggle Competitions
*Tech Stack: Python, PyTorch, Hugging Face Transformers, XGBoost, LightGBM, CatBoost, Scikit-learn*
- Benchmarked Linear Regression, Random Forest, XGBoost, LightGBM, and CatBoost for tabular price prediction, implementing feature engineering, cross-validation, and hyperparameter tuning to minimize validation error.
- Built an end-to-end PyTorch semantic segmentation pipeline (U-Net/DeepLab-style, Dice loss, IoU metric) for pixel-level classification and fine-tuned Hugging Face transformer models optimizing top-3 ranking via MAP@3.

---

## 🛠️ Technical Stack & Tooling

| Domain | Technologies & Libraries |
| :--- | :--- |
| **GenAI & Agentic Systems** | LangGraph, Model Context Protocol (MCP / FastMCP), ReAct Loop from Scratch, Hybrid RAG (Qdrant, BM25, RRF), Ragas, Rerankers (Cross-Encoder) |
| **Backend & Distributed** | FastAPI, Flask, REST APIs, Server-Sent Events (SSE), Pydantic v2, SQLAlchemy, Redis, Celery, JWT & RBAC |
| **Machine Learning & CV** | PyTorch, Hugging Face Transformers, YOLOv8, OpenCV, Scikit-learn, XGBoost, LightGBM, CatBoost, Pandas, NumPy |
| **Languages & Core CS** | Python, C/C++, Java, SQL, Data Structures & Algorithms, OOP, Database Management Systems |
| **DevOps & Developer Tools** | Git/GitHub, Docker, Linux, Postman, Pytest, Markdown |

---

## 🎓 Education

- **B.Tech in Computer Science and Engineering** — *Vellore Institute of Technology (VIT), Chennai* (2022 – 2026) &nbsp;|&nbsp; **CGPA: 7.93**
- **B.S. in Data Science and Applications** — *Indian Institute of Technology (IIT), Madras* (2022 – Present) &nbsp;|&nbsp; **CGPA: 6.49**
  - *Currently at Diploma level*
