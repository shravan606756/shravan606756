<div align="center">

<img src="banner.png" alt="Shravan Singh Udawat — Backend Engineer · Cloud-Native Systems · Applied AI" width="100%"/>

<p align="center">
  <a href="mailto:shravanudawat33@gmail.com"><img src="https://img.shields.io/badge/Email-shravanudawat33%40gmail.com-7a1f1f?style=for-the-badge&logo=gmail&logoColor=f5ecd7" alt="Email" /></a>
  <a href="https://www.linkedin.com/in/shravan-singh-udawat-5178aa337/"><img src="https://img.shields.io/badge/LinkedIn-Connect-7a1f1f?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
  <a href="https://leetcode.com/u/shravanudawat33/"><img src="https://img.shields.io/badge/LeetCode-Profile-FFA116?style=for-the-badge&logo=leetcode&logoColor=white" alt="LeetCode" /></a>
</p>

</div>

<br>

Building backend services and applied AI systems that hold up under real load: enterprise REST APIs on SQL/PostgreSQL backends, deterministic state machines for orchestration and recovery, simulation-guided decision agents, and embedding-based retrieval pipelines engineered for correctness and latency at scale.

I'm a Computer Science undergraduate at VIT Vellore, and most of what's below is a record of moving systems past the prototype stage replacing fragile, manual workflows with services that degrade gracefully and recover on their own.

<br>

## Experience

**BKT** — Software Engineering Summer Intern &nbsp;·&nbsp; *10 May 2026 – 30 June 2026*

Worked alongside SAP teams and business consultants to replace manual, repetitive aggregation queries with a robust API layer for internal sales analytics.

- Developed a Spring Boot backend exposing REST APIs over SQL Server data for recurring sales analytics.
- Wrote SQL Server stored procedures, functions, and triggers to support enterprise sales workflows.
- Validated OutSystems CRUD operations to protect data integrity across the platform.
- Built Power BI dashboards and SQL reports to monitor sales KPIs for business reporting.

<br>

## Featured Projects

**[ASTra](https://github.com/shravan606756/ASTra)** — A codebase comprehension tool that parses Java abstract syntax trees into a searchable, semantic index queried in plain English.
`Java 21` `Spring Boot` `PostgreSQL` `pgvector` `JavaParser` `LLMs`

<details>
<summary>View details</summary>
<br>

- Architected a Spring Boot REST service backed by PostgreSQL with the pgvector extension for approximate nearest-neighbor search over embedded code symbols.
- Built an adaptively batched, multithreaded indexing pipeline that reduced processing time by ~49% when parsing a 1,700+ class repository.
- Implemented semantic chunking and token-budget-aware context assembly to feed multiple LLM backends (OpenAI, Ollama, Groq), returning answers with exact line-level source references.
- Built a decoupled, interactive CLI client and an automated benchmarking suite to measure retrieval-quality and latency regressions.

</details>

<br>

**[Multi-Threaded DPI Engine](https://github.com/shravan606756/multi-threaded-dpi-engine)** — A high-performance network traffic analysis platform combining a multi-threaded C++ deep packet inspection engine with a Spring Boot orchestration backend and AI-powered insights.
`C++` `Spring Boot` `Redis` `Docker` `Llama 3`

<details>
<summary>View details</summary>
<br>

- Architected a multi-threaded C++ DPI engine with a load-balancer → fast-path worker pipeline, using five-tuple flow hashing to route packets deterministically and keep per-connection state race-free across threads.
- Built a layered packet-parsing pipeline (Ethernet/IP/TCP/UDP) with TLS SNI and HTTP host extraction to classify traffic by application and domain, applying rule-based blocking and emitting structured JSON analytics.
- Designed a Spring Boot orchestration layer that runs the native binary asynchronously via `ProcessBuilder`, with Redis-backed job-state and AI-response caching, and Groq (Llama 3.3-70B) generated traffic risk summaries.

</details>

<br>

**[ResilientDB](https://github.com/shravan606756/ResilientDB-Engine)** — A pluggable backup orchestration engine that decouples core scheduling logic from database-specific backup implementations.
`Java` `Spring Boot` `PostgreSQL` `AWS (EC2, RDS, ECR)` `Docker` `GitHub Actions`

<details>
<summary>View details</summary>
<br>

- Uses a Strategy Pattern-based engine supporting interchangeable PostgreSQL, MySQL, and MongoDB backup drivers without touching core orchestration code.
- Runs an asynchronous worker pool with exponential backoff retry logic to prevent HTTP thread-pool exhaustion during sustained backup load.
- Models job lifecycle as a deterministic finite state machine (PENDING → PROCESSING → COMPLETED/FAILED) with real-time health metrics, cutting mean time to recovery from hours to seconds.

</details>

<br>

## Other Projects

| Project | What it does | Stack |
|---|---|---|
| **[Eco-Looping Building Agent](https://github.com/shravan606756/eco-looping-building-agent)** | Closed-loop control system that optimizes HVAC energy consumption and occupant comfort through simulation-guided decision-making, with a Groq Llama 3.3 agent evaluating a matrix of simulated physical outcomes rather than fixed temperature heuristics. | `Python` `EnergyPlus` `Groq Llama 3.3` `Streamlit` `Pydantic` |
| **[TranscriptIQ](https://github.com/shravan606756/TranscriptIQ)** | Fault-tolerant audio intelligence pipeline turning long-form podcast transcripts into precisely retrievable answers, with a multi-tier ingestion pipeline cutting speech-to-text latency by 85% and FAISS + Llama-3.3 retrieval cutting search time by 65%. | `Python` `Transformers` `FAISS` `Whisper` `Llama-3 via Groq` |
| **[Email Writer Service](https://github.com/shravan606756/email-writer-springboot)** | Chrome extension that injects AI-generated, tone-controlled reply drafts directly into Gmail's compose UI via a stateless Spring Boot + Gemini API backend. | `Java` `Spring Boot` `React` `Chrome Extension` `Gemini API` |
| **[Hybrid Lexical-Semantic Matching](https://github.com/shravan606756/hybrid-lexical-semantic-matching)** | Interpretable NLP pipeline for candidate-role matching, combining TF-IDF lexical scoring with MiniLM embedding similarity and an explainability layer that surfaces top-contributing sentences behind each ranking. | `Python` `Scikit-learn` `Sentence Transformers` `Streamlit` |

<br>

## Technical Stack

**Languages**

![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![C](https://img.shields.io/badge/C-00599C?style=flat-square&logo=c&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=postgresql&logoColor=white)

**Frameworks & Libraries**

![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![REST APIs](https://img.shields.io/badge/REST_APIs-005571?style=flat-square)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white)
![Scikit-learn](https://img.shields.io/badge/Scikit_learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white)
![Pydantic](https://img.shields.io/badge/Pydantic-E92063?style=flat-square&logo=pydantic&logoColor=white)

**AI / ML**

![Transformers](https://img.shields.io/badge/Transformers-FFD21E?style=flat-square&logo=huggingface&logoColor=black)
![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=flat-square&logo=openai&logoColor=white)
![Groq](https://img.shields.io/badge/Groq-F55036?style=flat-square&logoColor=white)
![Gemini](https://img.shields.io/badge/Gemini-8E75B2?style=flat-square&logo=googlegemini&logoColor=white)
![FAISS](https://img.shields.io/badge/FAISS-7a1f1f?style=flat-square)
![Whisper](https://img.shields.io/badge/Whisper-7a1f1f?style=flat-square)
![Sentence Transformers](https://img.shields.io/badge/Sentence_Transformers-7a1f1f?style=flat-square)
![Vector Search](https://img.shields.io/badge/Vector_Search-7a1f1f?style=flat-square)

**Cloud & DevOps**

![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonaws&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![CI/CD](https://img.shields.io/badge/CI%2FCD-7a1f1f?style=flat-square)

**Databases**

![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=flat-square&logo=postgresql&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![pgvector](https://img.shields.io/badge/pgvector-316192?style=flat-square&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)

**Tools**

![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white)
![Postman](https://img.shields.io/badge/Postman-FF6C37?style=flat-square&logo=postman&logoColor=white)
![VS Code](https://img.shields.io/badge/VS_Code-007ACC?style=flat-square&logo=visualstudiocode&logoColor=white)
![IntelliJ IDEA](https://img.shields.io/badge/IntelliJ_IDEA-000000?style=flat-square&logo=intellijidea&logoColor=white)

<br>

## Certifications

<details>
<summary>View certifications (5)</summary>
<br>

**Microsoft Certified: Azure AI Engineer Associate** — Microsoft &nbsp;·&nbsp; Issued Jul 2025 · Expires Jul 2027

**Oracle Fusion AI Agent Studio Certified Foundations Associate** — Oracle &nbsp;·&nbsp; Issued Oct 2025

**Oracle Data Platform** — Oracle &nbsp;·&nbsp; Issued Oct 2025

**Oracle AI Cloud Infrastructure** — Oracle &nbsp;·&nbsp; Issued Oct 2025

**Oracle AI Foundation** — Oracle &nbsp;·&nbsp; Issued Oct 2025

</details>

<br>

<hr>

<div align="center">
<sub>Open to opportunities in backend engineering, and AI-integrated systems.</sub>
</div>
