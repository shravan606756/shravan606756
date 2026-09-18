<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:1a1a2e,100:0f3460&height=170&section=header&text=Shravan%20Singh%20Udawat&fontSize=40&fontColor=ffffff&animation=fadeIn&fontAlignY=38&desc=Backend%20Engineer%20%C2%B7%20RAG%20Systems%20%C2%B7%20Resilient%20Infrastructure&descAlignY=58&descSize=16&descColor=d0d0e0" width="100%"/>

<p align="center">
  <b>VIT Vellore &nbsp;·&nbsp; B.Tech Computer Science</b>
</p>

<p align="center">
  <a href="mailto:shravanudawat33@gmail.com"><img src="https://img.shields.io/badge/Email-shravanudawat33%40gmail.com-1a1a2e?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" /></a>
  <a href="https://www.linkedin.com/"><img src="https://img.shields.io/badge/LinkedIn-Connect-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
  <a href="https://github.com/"><img src="https://img.shields.io/badge/GitHub-Follow-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub" /></a>
  <a href="https://leetcode.com/u/shravanudawat33/"><img src="https://img.shields.io/badge/LeetCode-Profile-FFA116?style=for-the-badge&logo=leetcode&logoColor=white" alt="LeetCode" /></a>
</p>

<br>

> *Building the infrastructure other people defer: fault-tolerant pipelines, deterministic state machines, and retrieval systems that hold up under real load.*

</div>

<br>
<img src="https://capsule-render.vercel.app/api?type=rect&color=1a1a2e&height=2&section=header" width="100%"/>

## 👨‍💻 About Me

I am a final year Computer Science undergraduate at VIT Vellore, focused on backend systems, retrieval-augmented generation, and cloud-native infrastructure. My work centers on taking a system from a fragile prototype to something that survives real load, through fault-tolerant pipelines, deterministic state machines, and infrastructure that recovers from failure instead of collapsing under it.

<img src="https://capsule-render.vercel.app/api?type=rect&color=1a1a2e&height=2&section=header" width="100%"/>

## 💼 Experience

### BKT
**Software Engineering Summer Intern** &nbsp;·&nbsp; *May 10 2026 – June 30 2026*

Worked alongside SAP teams and business consultants to gather requirements and build an internal analytics backend that replaced manual, repetitive aggregation queries with a robust API layer.

- Developed a Spring Boot backend exposing 5 REST APIs over SQL Server data for recurring sales analytics.
- Wrote SQL Server stored procedures, functions, and triggers to support enterprise sales workflows.
- Validated OutSystems CRUD operations to protect data integrity across the platform.
- Built Power BI dashboards and SQL reports to monitor sales KPIs for business reporting.

<img src="https://capsule-render.vercel.app/api?type=rect&color=1a1a2e&height=2&section=header" width="100%"/>

## 🚀 Featured Projects

### ⚡ ResilientDB
`Java` `Spring Boot` `PostgreSQL` `AWS (EC2, RDS, ECR)` `Docker` `GitHub Actions`
> A pluggable backup orchestration engine built to eliminate core-logic coupling between database backends.
- Architected a pluggable engine using the Strategy Pattern for seamless PostgreSQL, MySQL, and MongoDB backup orchestration.
- Engineered an asynchronous worker pool with exponential backoff to suppress HTTP thread starvation under heavy load.
- Reduced MTTR from hours to seconds with a deterministic state machine (PENDING → PROCESSING → COMPLETED/FAILED) backed by real-time health metrics.

### ⚡ TranscriptIQ
`Python` `Transformers` `FAISS` `Whisper` `Llama-3 via Groq`
> A fault-tolerant audio intelligence pipeline that turns long podcast transcripts into precise, retrievable answers.
- Architected a multi-tier ingestion pipeline with prioritized transcript reuse and Whisper fallback, cutting STT latency by 85 percent.
- Solved long-context transformer limitations through boundary-aware chunking and a metrics-driven evaluation pipeline built in Streamlit to optimize BART/T5 inference.
- Designed a RAG-based QA system using FAISS retrieval and semantic embeddings with Llama-3.3, cutting information retrieval time by 65 percent.

### ⚡ [ASTra](https://github.com/shravan606756/ASTra)
`Java 21` `Spring Boot` `PostgreSQL` `pgvector` `JavaParser` `LLMs`
> A codebase comprehension tool that parses Java abstract syntax trees into a searchable, semantic index queried in plain English.
- Architected a Spring Boot REST service backed by PostgreSQL and pgvector for fast approximate nearest-neighbor (ANN) search over large codebases.
- Engineered an adaptively batched, multithreaded indexing pipeline that reduced processing time by ~49% when parsing a 1,700+ class repository.
- Designed a RAG pipeline with semantic chunking to feed LLMs (OpenAI, Ollama, Groq) under strict token budgets, delivering grounded answers with exact line-level source references.
- Built a decoupled, interactive CLI companion and integrated automated retrieval-quality benchmarks to validate intent-match accuracy and latency.

### ⚡ [Multi-Threaded DPI Engine](https://github.com/shravan606756/multi-threaded-dpi-engine)
`C++` `Spring Boot` `Redis` `Docker` `Llama 3`
> An end-to-end network traffic analysis system combining a high-performance C++ DPI engine with a Spring Boot orchestration backend and AI-powered insights.
- Developed a multi-threaded C++ Deep Packet Inspection engine utilizing hash-based load distribution for Five-Tuple flow tracking and TLS SNI extraction.
- Architected a Spring Boot orchestration layer featuring asynchronous execution via ProcessBuilder and Redis caching for job state management.
- Integrated the Groq API (Llama 3) to deliver automated, AI-powered traffic insights based on structured JSON analytics generated by the native C++ binary.
- Designed the system for scalable deployment across containerized environments using Docker and Docker Compose.

### ⚡ [Hybrid Lexical-Semantic Matching](https://github.com/shravan606756/hybrid-lexical-semantic-matching)
`Python` `NLP` `Scikit-learn` `Sentence Transformers` `Streamlit`
> An interpretable NLP pipeline for explainable candidate-role matching and deterministic skill-gap feedback.
- Built a multi-stage hybrid matching system that computes lexical relevance via TF-IDF vectorization and semantic similarity using MiniLM transformer embeddings.
- Engineered a hybrid scoring model with weighted linear aggregation to balance keyword precision with contextual meaning.
- Developed an explainability layer that justifies ranking decisions by surfacing top contributing sentences and generates deterministic improvement feedback based on extracted skill gaps.
- Deployed the end-to-end pipeline using Streamlit to facilitate interactive, small-batch resume screening and visualized analytics.

### ⚡ [Eco-Looping Building Agent](https://github.com/shravan606756/eco-looping-building-agent)
`Python` `EnergyPlus` `Groq Llama 3.3` `Streamlit` `Pydantic` `LLMs`[cite: 4]
> An AI-driven closed-loop orchestration engine that optimizes HVAC energy consumption and occupant comfort via a Simulation-Guided Agent Architecture[cite: 4].
- Engineered a stateless state-machine pipeline utilizing a custom ToolRegistry to decouple EnergyPlus physics simulations from the core LLM decision loop[cite: 4].
- Designed an empirical reasoning engine where a Groq Llama 3.3 agent evaluates a mathematical matrix of physical outcomes (energy usage, peak load, comfort) instead of relying on raw temperature rules[cite: 4].
- Implemented rigorous orchestration with Pydantic validation to ensure schema safety and built fault-tolerant diagnostic handling for subprocess C++ exit codes[cite: 4].
- Developed a real-time Streamlit dashboard to visualize iteration progression, convergence metrics, and energy savings reports[cite: 4].

### ⚡ [Email Writer Service](https://github.com/shravan606756/email-writer-springboot)
`Java` `Spring Boot` `GenAI` `REST API`
> An automated GenAI email orchestration tool.
- Developed a robust RESTful backend service for automated, context-aware email generation and templating.

<img src="https://capsule-render.vercel.app/api?type=rect&color=1a1a2e&height=2&section=header" width="100%"/>

## 🛠️ Technical Skills

<table>
  <tr>
    <td align="center" width="25%"><b>Languages</b></td>
    <td>
      <img src="https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white" />
      <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" />
      <img src="https://img.shields.io/badge/C-00599C?style=flat-square&logo=c&logoColor=white" />
      <img src="https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=mysql&logoColor=white" />
    </td>
  </tr>
  <tr>
    <td align="center" width="25%"><b>Backend & Databases</b></td>
    <td>
      <img src="https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white" />
      <img src="https://img.shields.io/badge/REST_APIs-005571?style=flat-square&logo=fastapi&logoColor=white" />
      <img src="https://img.shields.io/badge/PostgreSQL-316192?style=flat-square&logo=postgresql&logoColor=white" />
      <img src="https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white" />
      <img src="https://img.shields.io/badge/Postman-FF6C37?style=flat-square&logo=postman&logoColor=white" />
    </td>
  </tr>
  <tr>
    <td align="center" width="25%"><b>Data & AI</b></td>
    <td>
      <img src="https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white" />
      <img src="https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white" />
      <img src="https://img.shields.io/badge/RAG-1a1a2e?style=flat-square" />
      <img src="https://img.shields.io/badge/Vector_DBs-1a1a2e?style=flat-square" />
      <img src="https://img.shields.io/badge/Sentence_Transformers-1a1a2e?style=flat-square" />
    </td>
  </tr>
  <tr>
    <td align="center" width="25%"><b>Cloud & DevOps</b></td>
    <td>
      <img src="https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonaws&logoColor=white" />
      <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" />
      <img src="https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white" />
      <img src="https://img.shields.io/badge/CI%2FCD-1a1a2e?style=flat-square" />
    </td>
  </tr>
  <tr>
    <td align="center" width="25%"><b>Tools</b></td>
    <td>
      <img src="https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white" />
      <img src="https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white" />
      <img src="https://img.shields.io/badge/VS_Code-007ACC?style=flat-square&logo=visualstudiocode&logoColor=white" />
      <img src="https://img.shields.io/badge/IntelliJ_IDEA-000000?style=flat-square&logo=intellijidea&logoColor=white" />
    </td>
  </tr>
</table>

<br>

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:1a1a2e,100:0f3460&height=120&section=footer" width="100%"/>

<sub>Open to opportunities in backend engineering, machine learning, and AI-integrated systems.</sub>

</div>
