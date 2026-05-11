<h1 align="center">Hi, I'm Aryan Shah 👋</h1>
<h3 align="center">ML Engineer · RAG Systems · Full-Stack AI Applications</h3>

<p align="center">
  <a href="https://linkedin.com/in/aryan-shah-3674031ba"><img src="https://img.shields.io/badge/LinkedIn-%230077B5.svg?style=for-the-badge&logo=linkedin&logoColor=white"/></a>
  <a href="mailto:aryanrshah2109@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white"/></a>
  <a href="https://x.com/Aryan54578157"><img src="https://img.shields.io/badge/X-black.svg?style=for-the-badge&logo=X&logoColor=white"/></a>
  <a href="https://instagram.com/aryan_shah21"><img src="https://img.shields.io/badge/Instagram-%23E4405F.svg?style=for-the-badge&logo=Instagram&logoColor=white"/></a>
</p>

---

## About Me

I build end-to-end AI systems with a focus on retrieval-augmented generation, semantic search, and production ML pipelines. My work spans the full stack — from AST-based code chunkers and hybrid vector retrieval backends to Streamlit and React frontends.

- 🔭 Currently building **GitExplore** — a RAG system for natural language Q&A over GitHub repositories
- 🌱 Deep-diving into **LLMs, agentic AI workflows, hybrid search, and MLOps**
- 💬 Ask me about **RAG architecture, hybrid retrieval (BM25 + dense), AST chunking, or ML deployment**
- ⚡ I love building tools that automate my own problems — then turning them into full projects

---

## Featured Projects

### 🔍 GitExplore
> **Natural language Q&A over any GitHub repository using RAG**

Point GitExplore at any public GitHub repo and ask questions in plain English. The system clones the repo, parses source files into semantically meaningful chunks using AST analysis, embeds them into a hybrid search index, and returns precise, source-attributed answers.

**Key engineering decisions:**
- **AST-based chunking** via tree-sitter — treats each function and class as an atomic unit rather than splitting at arbitrary token windows. Supports Python, JavaScript, TypeScript, Java, Go, and Rust.
- **Hybrid retrieval** combining BM25 sparse search (exact token matching for function names, imports) with dense vector embeddings (semantic similarity) fused via Reciprocal Rank Fusion
- **Query type routing** — classifies queries into `explain_code`, `find_function`, `debug`, and `architecture` types and adapts retrieval strategy and prompt template per type
- **Source attribution** on every response — file path, function name, and line numbers cited inline

**Stack:** Python · FastAPI · Qdrant · BM25 (rank_bm25) · voyage-code-2 · Ollama (mistral:7b) · tree-sitter · Streamlit

---

### 🎓 ExamEcho
> **AI-powered viva and interview evaluation platform with voice interaction**

ExamEcho simulates real examination environments — conducting voice-based viva and interview sessions, evaluating student responses with AI, and delivering structured examiner-like feedback. Built to eliminate the subjectivity, inconsistency, and limited scalability of traditional manual evaluations.

**Key features:**
- AI-generated questions that are module-wise, topic-specific, and difficulty-controlled
- Voice interaction via Speech-to-Text (student answers) and Text-to-Speech (question delivery)
- Automated evaluation scoring answers on correctness, clarity, completeness, and communication
- Adaptive follow-up questions generated dynamically based on student responses
- Performance analytics dashboard for both students and educators

Selected for **SSIP (Student Startup and Innovation Policy) funding** by the Gujarat government.

**Stack:** Python · FastAPI · React · Speech-to-Text · Text-to-Speech · LLM APIs · Cloud

---

### 🛡️ FraudDetect
> **Production-grade ML system for real-time credit card fraud detection**

An end-to-end fraud detection system built with MLOps best practices — covering data ingestion, feature engineering, model training with GPU acceleration, threshold optimization, and a real-time REST API with sub-100ms inference latency. Deployed and live.

**Key engineering details:**
- XGBoost classifier (263 estimators, CUDA-accelerated) with precision-constrained threshold optimization — maximizes recall subject to ≥65% precision
- Domain-aware feature engineering including balance error detection (`|amount - balance_delta|`) to catch transaction anomalies
- Full MLOps stack: MLflow experiment tracking, DVC data versioning, timestamped artifact storage, DagHub remote tracking server
- Handles severe class imbalance via `scale_pos_weight=7.45` with stratified splits and PR-AUC as the primary eval metric

**Stack:** Python · XGBoost · FastAPI · scikit-learn · MLflow · DVC · Docker · Vanilla JS frontend

**Live:** [API](https://frauddetect-backend-jpgf.onrender.com/docs) · [App](https://frauddetect-1gju.onrender.com/)

---

## Tech Stack

**Languages**

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=for-the-badge&logo=javascript&logoColor=%23F7DF1E)
![Java](https://img.shields.io/badge/java-%23ED8B00.svg?style=for-the-badge&logo=openjdk&logoColor=white)
![C](https://img.shields.io/badge/c-%2300599C.svg?style=for-the-badge&logo=c&logoColor=white)

**AI / ML**

![PyTorch](https://img.shields.io/badge/PyTorch-%23EE4C2C.svg?style=for-the-badge&logo=PyTorch&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-%23FF6F00.svg?style=for-the-badge&logo=TensorFlow&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Keras](https://img.shields.io/badge/Keras-%23D00000.svg?style=for-the-badge&logo=Keras&logoColor=white)
![OpenCV](https://img.shields.io/badge/opencv-%23white.svg?style=for-the-badge&logo=opencv&logoColor=white)
![mlflow](https://img.shields.io/badge/mlflow-%23d9ead3.svg?style=for-the-badge&logo=numpy&logoColor=blue)

**Backend & APIs**

![FastAPI](https://img.shields.io/badge/FastAPI-005571?style=for-the-badge&logo=fastapi)
![Express.js](https://img.shields.io/badge/express.js-%23404d59.svg?style=for-the-badge&logo=express&logoColor=%2361DAFB)

**Frontend**

![React](https://img.shields.io/badge/react-%2320232a.svg?style=for-the-badge&logo=react&logoColor=%2361DAFB)
![Streamlit](https://img.shields.io/badge/Streamlit-%23FE4B4B.svg?style=for-the-badge&logo=streamlit&logoColor=white)
![Bootstrap](https://img.shields.io/badge/bootstrap-%238511FA.svg?style=for-the-badge&logo=bootstrap&logoColor=white)

**Databases & Vector Stores**

![Postgres](https://img.shields.io/badge/postgres-%23316192.svg?style=for-the-badge&logo=postgresql&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-%234ea94b.svg?style=for-the-badge&logo=mongodb&logoColor=white)
![MySQL](https://img.shields.io/badge/mysql-4479A1.svg?style=for-the-badge&logo=mysql&logoColor=white)
![SQLite](https://img.shields.io/badge/sqlite-%2307405e.svg?style=for-the-badge&logo=sqlite&logoColor=white)

**Infrastructure & DevOps**

![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-%23FF9900.svg?style=for-the-badge&logo=amazon-aws&logoColor=white)
![Google Cloud](https://img.shields.io/badge/GoogleCloud-%234285F4.svg?style=for-the-badge&logo=google-cloud&logoColor=white)
![Azure](https://img.shields.io/badge/azure-%230072C6.svg?style=for-the-badge&logo=microsoftazure&logoColor=white)
![Git](https://img.shields.io/badge/git-%23F05033.svg?style=for-the-badge&logo=git&logoColor=white)

---

## Currently Learning

- Advanced RAG patterns: hybrid retrieval, reranking, dependency graph expansion
- Agentic AI workflows and multi-step reasoning pipelines
- MLOps: model serving, monitoring, and deployment at scale

---
