# Bharanee B

### GenAI and Agentic Systems | Computer Vision and Multimodal Systems | Backend Engineering
**B.Tech Computer Science @ VIT Chennai** | **B.S. Data Science and Applications @ IIT Madras**

[LinkedIn](https://www.linkedin.com/in/bharanee-b-a387902b5/) | [GitHub](https://github.com/Totto1403) | bharanee1403@gmail.com

---

Software engineer and researcher specializing in production-grade **Agentic AI systems**, real-time **computer vision and multimodal perception**, and resilient **distributed backend infrastructure**. Experienced in designing technical systems end-to-end: from mathematical formulation, custom temporal feature engineering, and model evaluation to low-latency streaming APIs, event-driven task queues, and autonomous agent execution loops.

---

## Technical Competencies

| Domain | Technologies and Frameworks |
| :--- | :--- |
| **GenAI and Agentic Systems** | LangGraph, Model Context Protocol (MCP / FastMCP), Autonomous ReAct Loops, Hybrid RAG (Qdrant, BM25, RRF), Cross-Encoder Reranking, Ragas / DeepEval |
| **Computer Vision and Multimodal AI** | PyTorch, MediaPipe (Face Mesh, Pose), OpenCV, YOLOv8, ResNet-34, Perspective-n-Point (solvePnP), Multimodal Late Fusion |
| **Backend and Distributed Systems** | FastAPI, Flask Blueprints, RESTful APIs, Server-Sent Events (SSE), Pydantic v2, SQLAlchemy, Redis Caching, Celery Task Queues, JWT and RBAC |
| **Applied Machine Learning** | Scikit-learn, XGBoost, LightGBM, CatBoost, Hugging Face Transformers, Time-Series Feature Engineering, Pandas, NumPy |
| **Languages and Core CS** | Python, C/C++, Java, SQL, JavaScript, HTML/CSS, Data Structures and Algorithms, Object-Oriented Design, Relational Database Management |
| **Developer Tools and Deployment** | Git/GitHub, Docker, Linux, Postman, Pytest, Markdown |

---

## Featured Systems and Engineering Projects

### [Enterprise Multi-Agent Intelligence Engine](https://github.com/Totto1403/multiagent-mcp-rag)
*Tech Stack: Python 3.11+, LangGraph, FastMCP (Model Context Protocol), Qdrant, BM25, FastAPI, Pydantic v2, SQLite, Ragas*
- Architected an asynchronous multi-agent enterprise platform orchestrating Supervisor routing, self-correcting NL-to-SQL generation, and citation-grounded Hybrid RAG over financial transaction databases and credit policy documents.
- Built a two-stage retrieval pipeline fusing dense vector search (Qdrant 1536d) and sparse keyword retrieval (BM25 Okapi) via Reciprocal Rank Fusion (RRF, $k=60$) with Cross-Encoder reranking, achieving 100% Context Precision (Rank-1 retrieval) across all evaluated queries.
- Decoupled tool execution services via FastMCP supporting dual transports (low-latency Stdio subprocesses and distributed SSE over HTTP) with AST-level SQL validation (`sqlparse`) blocking mutations, URI read-only engine locks, and automated query rewriting on syntax errors.
- Implemented real-time token and intermediate thought streaming via FastAPI Server-Sent Events (SSE) guarded by Pydantic schemas, recording a 98.8% composite benchmark evaluation score and a 9.0ms median end-to-end latency (p50).

### [MicroAgent: Zero-Framework Single-Agent ReAct Engine From Scratch](https://github.com/Totto1403/microagent-from-scratch)
*Tech Stack: Python 3.10+, Autonomous ReAct Loop, Pydantic v2, OpenAI API, Rich, Pytest*
- Engineered a transparent, zero-framework autonomous AI agent from scratch in pure Python to eliminate third-party framework overhead and master raw agentic execution loops.
- Implemented an AST-inspected `@tool` decorator that dynamically translates native Python function signatures, docstrings, and type annotations into strict OpenAPI/JSON function specifications.
- Built an adaptive self-healing execution loop that intercepts runtime exceptions, syntax errors, and missing file faults into structured diagnostic observations, enabling autonomous LLM self-correction.
- Integrated sliding-window context pruning with token estimation, sandboxed Python REPL and AST calculator tools, interactive Human-in-the-Loop (HITL) approval gates, and a comprehensive offline test suite powered by `MockLLMClient`.

### Driver Risk Assessment System (DRAS) - Final-Year Capstone
*Tech Stack: Python, PyTorch, OpenCV, YOLOv8, ResNet-34, Scikit-learn*
- Engineered an edge-deployable multimodal safety pipeline concurrently monitoring 4 perception channels: physical fatigue, affective state, postural deviation, and visual-manual distraction into a single continuous risk score.
- Integrated continuous Exponentially Weighted Moving Average (EWMA) baseline calibration for Eye Aspect Ratio (EAR) thresholds, eliminating false positives caused by static cutoffs without requiring manual user setup.
- Fine-tuned a ResNet-34 classifier on FER2013 using Focal Loss ($\gamma = 2.0$) and cosine annealing to achieve 70.24% accuracy on unseen test data, incorporating a 10-frame temporal majority vote to suppress facial jitter.
- Designed an empirical 70:30 visual-behavioral to affective late-fusion scoring model grounded in naturalistic driving research (SHRP 2), enforcing an 85% hard risk floor on YOLOv8n mobile phone detection.
- Trained a temporal Random Forest classifier with 20 engineered time-series features over a 30-frame sliding window on the NTHU-DDD benchmark (65,708 test frames, 36 subjects), achieving **93.17% accuracy, 94.52% recall, and 98.09% AUC-ROC**, significantly outperforming the published 90.48% baseline.

### Study Optimizer: Mood and Posture-Based Engagement Feedback System
*Tech Stack: Python, PyTorch, MediaPipe Face Mesh, MediaPipe Pose, ResNet-34, OpenCV*
- Designed an intelligent, non-intrusive e-learning companion that tracks facial affect, head pose, eye vigilance (EAR), and seated posture in real time via consumer webcam.
- Built a stateful engagement logic engine with persistent time-based counters (`distracted_counter`, `bad_posture_counter`, `eye_closed_counter`) to distinguish brief natural movements from chronic disengagement.
- Implemented a composite Study Optimizer Score (SOS) weighting mood (0.45), posture (0.25), focus (0.15), and vigilance (0.15), complete with a 3-tier hierarchical alert system and automated "Take a Break" meta-alerts.
- Validated through empirical user trials, demonstrating an 83.3% reduction in posture alerts and a 57.1% decrease in distraction events during monitored study sessions.

### [Placement Portal Application](https://github.com/Totto1403/placement_portal_app_v2_22f2000805)
*Tech Stack: Python, Flask Blueprints, Vue.js 3, Redis, Celery, JWT, SQLAlchemy, SQLite*
- Engineered a decoupled recruitment portal with JWT-authenticated Role-Based Access Control (RBAC) supporting distinct workflows for Institute Admins, Recruiting Companies, and Students.
- Integrated Redis caching and asynchronous Celery background workers to handle high-latency jobs (such as candidate CSV report exports) and prevent bottlenecking on high-traffic job boards.
- Built a modular single-page frontend using Vue.js 3 and Vite, configured with Progressive Web App (PWA) capabilities for multi-device deployment.

---

## Competitive Machine Learning and Benchmark Modeling

Practical implementations across competitive data science assignments, national programming practice exams, and Kaggle benchmarks:

- **Heavy Equipment Selling Price Prediction**: Engineered tabular regression pipelines on high-cardinality multi-modal industrial equipment records. Benchmarked Linear Regression, Random Forest, XGBoost, LightGBM, and CatBoost, optimizing hyperparameters and cross-validation against the Root Mean Squared Logarithmic Error (RMSLE) metric.
- **Hardware Parts Semantic Segmentation**: Built an end-to-end PyTorch semantic segmentation pipeline (U-Net and DeepLab architectures) to segment and classify six cluttered hardware components (hex nuts, washers, bolts, bearings, springs, o-rings) across 2,000 training and 500 test images. Optimized using Dice coefficient loss and column-major Run-Length Encoding (RLE).
- **Smart MCQ Solver Challenge**: Developed deep learning question-answering systems to predict and rank top-3 probable answers for multi-choice prompts, optimizing models against Mean Average Precision at 3 (MAP@3).
- **ECG Heartbeat Arrhythmia Classification**: Implemented 1D time-series classification models to categorize individual hospital ECG signals into four clinical arrhythmia categories, maximizing Macro F1-Score across imbalanced heartbeat distributions.
- **Customer Churn and Ticket Price Benchmarks**: Built supervised classification pipelines predicting customer exit status evaluated on F1-Score, regression models predicting flight ticket pricing evaluated on R2-Score, and mushroom edibility classification on categorical data.

---

## Education

- **Bachelor of Technology (B.Tech) in Computer Science and Engineering**
  *Vellore Institute of Technology (VIT), Chennai* | 2022 - 2026
  - CGPA: 7.93

- **Bachelor of Science (B.S.) in Data Science and Applications**
  *Indian Institute of Technology (IIT), Madras* | 2022 - Present
  - Currently at Diploma level | CGPA: 6.49
