<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:1a1a2e,100:0f3460&height=170&section=header&text=Shravan%20Singh%20Udawat&fontSize=40&fontColor=ffffff&animation=fadeIn&fontAlignY=38&desc=Backend%20Engineer%20%C2%B7%20Cloud-Native%20Systems%20%C2%B7%20Applied%20AI%20Agents&descAlignY=58&descSize=16&descColor=d0d0e0" width="100%"/>

<p align="center">
  <a href="mailto:shravanudawat33@gmail.com"><img src="https://img.shields.io/badge/Email-shravanudawat33%40gmail.com-1a1a2e?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" /></a>
  <a href="https://www.linkedin.com/"><img src="https://img.shields.io/badge/LinkedIn-Connect-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
  <a href="https://github.com/"><img src="https://img.shields.io/badge/GitHub-Follow-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub" /></a>
  <a href="https://leetcode.com/u/shravanudawat33/"><img src="https://img.shields.io/badge/LeetCode-Profile-FFA116?style=for-the-badge&logo=leetcode&logoColor=white" alt="LeetCode" /></a>
</p>

</div>

<br>

Building backend services and applied AI systems that hold up under real load: enterprise REST APIs on SQL/PostgreSQL backends, deterministic state machines for orchestration and recovery, simulation-guided decision agents, and embedding-based retrieval pipelines engineered for correctness and latency at scale.

I'm a Computer Science undergraduate at VIT Vellore, and most of what's below is a record of moving systems past the prototype stage — replacing fragile, manual workflows with services that degrade gracefully and recover on their own.

<br>

## Experience

**BKT** — Software Engineering Summer Intern &nbsp;·&nbsp; *10 May 2026 – 30 June 2026*

Worked alongside SAP teams and business consultants to replace manual, repetitive aggregation queries with a robust API layer for internal sales analytics.

- Developed a Spring Boot backend exposing REST APIs over SQL Server data for recurring sales analytics.
- Wrote SQL Server stored procedures, functions, and triggers to support enterprise sales workflows.
- Validated OutSystems CRUD operations to protect data integrity across the platform.
- Built Power BI dashboards and SQL reports to monitor sales KPIs for business reporting.

<br>

## Projects

**[ASTra](https://github.com/shravan606756/ASTra)** — A codebase comprehension tool that parses Java abstract syntax trees into a searchable, semantic index queried in plain English.
`Java 21` `Spring Boot` `PostgreSQL` `pgvector` `JavaParser` `LLMs`
- Architected a Spring Boot REST service backed by PostgreSQL with the pgvector extension for approximate nearest-neighbor search over embedded code symbols.
- Built an adaptively batched, multithreaded indexing pipeline that reduced processing time by ~49% when parsing a 1,700+ class repository.
- Implemented semantic chunking and token-budget-aware context assembly to feed multiple LLM backends (OpenAI, Ollama, Groq), returning answers with exact line-level source references.
- Built a decoupled, interactive CLI client and an automated benchmarking suite to measure retrieval-quality and latency regressions.

**[Eco-Looping Building Agent](https://github.com/shravan606756/eco-looping-building-agent)** — A closed-loop control system that optimizes HVAC energy consumption and occupant comfort through simulation-guided decision-making.
`Python` `EnergyPlus` `Groq Llama 3.3` `Streamlit` `Pydantic` `LLMs`
- Built a stateless pipeline using a custom tool registry to decouple EnergyPlus physics simulations from the core decision-making loop.
- Designed a decision engine where a Groq Llama 3.3 agent evaluates a matrix of simulated physical outcomes (energy usage, peak load, comfort) rather than applying fixed temperature heuristics.
- Enforced schema safety with Pydantic validation across the orchestration layer and built fault-tolerant handling for subprocess exit codes from the C++ simulation engine.
- Built a real-time Streamlit dashboard to visualize iteration progression, convergence metrics, and energy savings.

**[TranscriptIQ](https://github.com/shravan606756/TranscriptIQ)** — A fault-tolerant audio intelligence pipeline that converts long-form podcast transcripts into precisely retrievable answers.
`Python` `Transformers` `FAISS` `Whisper` `Llama-3 via Groq`
- Designed a multi-tier ingestion pipeline with prioritized transcript-cache reuse and Whisper-based transcription fallback, reducing speech-to-text latency by 85%.
- Addressed transformer context-length constraints through boundary-aware text chunking and a metrics-driven Streamlit evaluation harness for tuning BART/T5 summarization inference.
- Built a question-answering system combining FAISS approximate nearest-neighbor search over sentence embeddings with Llama-3.3 for context-grounded response generation, cutting information retrieval time by 65%.

**[ResilientDB](https://github.com/shravan606756/ResilientDB-Engine)** — A pluggable backup orchestration engine that decouples core scheduling logic from database-specific backup implementations.
`Java` `Spring Boot` `PostgreSQL` `AWS (EC2, RDS, ECR)` `Docker` `GitHub Actions`
- Architected a Strategy Pattern-based engine supporting interchangeable PostgreSQL, MySQL, and MongoDB backup drivers without touching core orchestration code.
- Built an asynchronous worker pool with exponential backoff retry logic to prevent HTTP thread-pool exhaustion during sustained backup load.
- Modeled job lifecycle as a deterministic finite state machine (PENDING → PROCESSING → COMPLETED/FAILED) with real-time health metrics, cutting mean time to recovery from hours to seconds.

**[Multi-Threaded DPI Engine](https://github.com/shravan606756/multi-threaded-dpi-engine)** — An end-to-end network traffic analysis system combining a high-performance C++ deep packet inspection engine with a Spring Boot orchestration backend.
`C++` `Spring Boot` `Redis` `Docker` `Llama 3`
- Built a multi-threaded C++ deep packet inspection engine using hash-based load distribution for five-tuple flow tracking and TLS SNI extraction.
- Architected a Spring Boot orchestration layer with asynchronous process execution via ProcessBuilder and Redis-backed job state caching.
- Integrated the Groq API (Llama 3) to generate automated traffic insight summaries from structured JSON analytics produced by the native C++ binary.
- Packaged the system for containerized deployment with Docker and Docker Compose.

**[Email Writer Service](https://github.com/shravan606756/email-writer-springboot)** — A Chrome extension that injects AI-generated reply controls directly into Gmail's compose UI, backed by a Spring Boot service.
`Java` `Spring Boot` `React` `Chrome Extension` `Gemini API` `REST API`
- Built a Spring Boot REST backend that integrates the Gemini API to generate email replies conditioned on the original message content.
- Designed a mood-based generation system letting users select a tone (e.g. formal, casual, assertive) that is injected into the prompt to steer the generated reply's style.
- Built a Chrome extension using React components injected into the Gmail DOM to render reply-generation buttons directly within the existing compose window, avoiding a separate standalone UI.
- Structured the client-server integration around a stateless REST API, keeping the extension lightweight and the generation logic centralized on the backend.

**[Hybrid Lexical-Semantic Matching](https://github.com/shravan606756/hybrid-lexical-semantic-matching)** — An interpretable NLP pipeline for explainable candidate-role matching and deterministic skill-gap feedback.
`Python` `NLP` `Scikit-learn` `Sentence Transformers` `Streamlit`
- Built a multi-stage matching system combining TF-IDF-based lexical relevance scoring with MiniLM transformer embedding similarity.
- Designed a weighted linear aggregation model to balance keyword precision against contextual semantic similarity.
- Built an explainability layer that surfaces the top contributing sentences behind each ranking decision and generates deterministic, skill-gap-driven improvement feedback.
- Deployed the pipeline as an interactive Streamlit application for small-batch resume screening with visualized analytics.

<br>

## Technical Stack

**Languages**

![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![C](https://img.shields.io/badge/C-00599C?style=for-the-badge&logo=c&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=postgresql&logoColor=white)

**Frameworks & Libraries**

![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![REST APIs](https://img.shields.io/badge/REST_APIs-005571?style=for-the-badge)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white)
![Scikit-learn](https://img.shields.io/badge/Scikit_learn-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white)
![Pydantic](https://img.shields.io/badge/Pydantic-E92063?style=for-the-badge&logo=pydantic&logoColor=white)

**AI / ML**

![Transformers](https://img.shields.io/badge/Transformers-FFD21E?style=for-the-badge&logo=huggingface&logoColor=black)
![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=for-the-badge&logo=openai&logoColor=white)
![Groq](https://img.shields.io/badge/Groq-F55036?style=for-the-badge&logoColor=white)
![Gemini](https://img.shields.io/badge/Gemini-8E75B2?style=for-the-badge&logo=googlegemini&logoColor=white)
![FAISS](https://img.shields.io/badge/FAISS-1a1a2e?style=for-the-badge)
![Whisper](https://img.shields.io/badge/Whisper-1a1a2e?style=for-the-badge)
![Sentence Transformers](https://img.shields.io/badge/Sentence_Transformers-1a1a2e?style=for-the-badge)
![Vector Search](https://img.shields.io/badge/Vector_Search-1a1a2e?style=for-the-badge)

**Cloud & DevOps**

![AWS](https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazonaws&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white)
![CI/CD](https://img.shields.io/badge/CI%2FCD-1a1a2e?style=for-the-badge)

**Databases**

![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![pgvector](https://img.shields.io/badge/pgvector-316192?style=for-the-badge&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white)

**Tools**

![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)
![Postman](https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=postman&logoColor=white)
![VS Code](https://img.shields.io/badge/VS_Code-007ACC?style=for-the-badge&logo=visualstudiocode&logoColor=white)
![IntelliJ IDEA](https://img.shields.io/badge/IntelliJ_IDEA-000000?style=for-the-badge&logo=intellijidea&logoColor=white)

<br>

## Certifications

**Microsoft Certified: Azure AI Engineer Associate** — Microsoft &nbsp;·&nbsp; Issued Jul 2025 · Expires Jul 2027

**Oracle Fusion AI Agent Studio Certified Foundations Associate** — Oracle &nbsp;·&nbsp; Issued Oct 2025

**Oracle Data Platform** — Oracle &nbsp;·&nbsp; Issued Oct 2025

**Oracle AI Cloud Infrastructure** — Oracle &nbsp;·&nbsp; Issued Oct 2025

**Oracle AI Foundation** — Oracle &nbsp;·&nbsp; Issued Oct 2025

<br>

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:1a1a2e,100:0f3460&height=120&section=footer" width="100%"/>

<sub>Open to opportunities in backend engineering, machine learning, and AI-integrated systems.</sub>

</div>
