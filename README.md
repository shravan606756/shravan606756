<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:1a1a2e,100:0f3460&height=170&section=header&text=Shravan%20Singh%20Udawat&fontSize=40&fontColor=ffffff&animation=fadeIn&fontAlignY=38&desc=Backend%20Engineer%20%C2%B7%20Cloud-Native%20Systems%20%C2%B7%20Applied%20AI%20Agents&descAlignY=58&descSize=16&descColor=d0d0e0" width="100%"/>

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

> Building backend services and applied AI systems that hold up under real load: enterprise REST APIs on SQL/PostgreSQL backends, deterministic state machines for orchestration and recovery, simulation-guided decision agents, and embedding-based retrieval pipelines engineered for correctness and latency at scale.

</div>

<br>
<img src="https://capsule-render.vercel.app/api?type=rect&color=1a1a2e&height=2&section=header" width="100%"/>

## About Me

I am a final-year Computer Science undergraduate at VIT Vellore, focused on backend systems, applied generative AI, and cloud-native infrastructure. My work centers on taking a system from a fragile prototype to something that survives production load, through fault-tolerant pipelines, deterministic state machines, and infrastructure that recovers from failure instead of collapsing under it.

<img src="https://capsule-render.vercel.app/api?type=rect&color=1a1a2e&height=2&section=header" width="100%"/>

## Experience

### BKT
**Software Engineering Summer Intern** &nbsp;·&nbsp; *10 May 2026 – 30 June 2026*

Worked alongside SAP teams and business consultants to gather requirements and build an internal analytics backend that replaced manual, repetitive aggregation queries with a robust API layer.

- Developed a Spring Boot backend exposing 5 REST APIs over SQL Server data for recurring sales analytics.
- Wrote SQL Server stored procedures, functions, and triggers to support enterprise sales workflows.
- Validated OutSystems CRUD operations to protect data integrity across the platform.
- Built Power BI dashboards and SQL reports to monitor sales KPIs for business reporting.

<img src="https://capsule-render.vercel.app/api?type=rect&color=1a1a2e&height=2&section=header" width="100%"/>

## Featured Projects

### [ASTra](https://github.com/shravan606756/ASTra)
`Java 21` `Spring Boot` `PostgreSQL` `pgvector` `JavaParser` `LLMs`
> A codebase comprehension tool that parses Java abstract syntax trees into a searchable, semantic index queried in plain English.
- Architected a Spring Boot REST service backed by PostgreSQL with the pgvector extension for approximate nearest-neighbor search over embedded code symbols.
- Built an adaptively batched, multithreaded indexing pipeline that reduced processing time by ~49% when parsing a 1,700+ class repository.
- Implemented semantic chunking and token-budget-aware context assembly to feed multiple LLM backends (OpenAI, Ollama, Groq), returning answers with exact line-level source references.
- Built a decoupled, interactive CLI client and an automated benchmarking suite to measure retrieval-quality and latency regressions.

### [Eco-Looping Building Agent](https://github.com/shravan606756/eco-looping-building-agent)
`Python` `EnergyPlus` `Groq Llama 3.3` `Streamlit` `Pydantic` `LLMs`
> A closed-loop control system that optimizes HVAC energy consumption and occupant comfort through simulation-guided decision-making.
- Built a stateless pipeline using a custom tool registry to decouple EnergyPlus physics simulations from the core decision-making loop.
- Designed a decision engine where a Groq Llama 3.3 agent evaluates a matrix of simulated physical outcomes (energy usage, peak load, comfort) rather than applying fixed temperature heuristics.
- Enforced schema safety with Pydantic validation across the orchestration layer and built fault-tolerant handling for subprocess exit codes from the C++ simulation engine.
- Built a real-time Streamlit dashboard to visualize iteration progression, convergence metrics, and energy savings.

### [TranscriptIQ](https://github.com/shravan606756/TranscriptIQ)
`Python` `Transformers` `FAISS` `Whisper` `Llama-3 via Groq`
> A fault-tolerant audio intelligence pipeline that converts long-form podcast transcripts into precisely retrievable answers.
- Designed a multi-tier ingestion pipeline with prioritized transcript-cache reuse and Whisper-based transcription fallback, reducing speech-to-text latency by 85%.
- Addressed transformer context-length constraints through boundary-aware text chunking and a metrics-driven Streamlit evaluation harness for tuning BART/T5 summarization inference.
- Built a question-answering system combining FAISS approximate nearest-neighbor search over sentence embeddings with Llama-3.3 for context-grounded response generation, cutting information retrieval time by 65%.

### [ResilientDB](https://github.com/shravan606756/ResilientDB-Engine)
`Java` `Spring Boot` `PostgreSQL` `AWS (EC2, RDS, ECR)` `Docker` `GitHub Actions`
> A pluggable backup orchestration engine that decouples core scheduling logic from database-specific backup implementations.
- Architected a Strategy Pattern-based engine supporting interchangeable PostgreSQL, MySQL, and MongoDB backup drivers without touching core orchestration code.
- Built an asynchronous worker pool with exponential backoff retry logic to prevent HTTP thread-pool exhaustion during sustained backup load.
- Modeled job lifecycle as a deterministic finite state machine (PENDING → PROCESSING → COMPLETED/FAILED) with real-time health metrics, cutting mean time to recovery from hours to seconds.

### [Multi-Threaded DPI Engine](https://github.com/shravan606756/multi-threaded-dpi-engine)
`C++` `Spring Boot` `Redis` `Docker` `Llama 3`
> An end-to-end network traffic analysis system combining a high-performance C++ deep packet inspection engine with a Spring Boot orchestration backend.
- Built a multi-threaded C++ deep packet inspection engine using hash-based load distribution for five-tuple flow tracking and TLS SNI extraction.
- Architected a Spring Boot orchestration layer with asynchronous process execution via ProcessBuilder and Redis-backed job state caching.
- Integrated the Groq API (Llama 3) to generate automated traffic insight summaries from structured JSON analytics produced by the native C++ binary.
- Packaged the system for containerized deployment with Docker and Docker Compose.

### [Email Writer Service](https://github.com/shravan606756/email-writer-springboot)
`Java` `Spring Boot` `React` `Chrome Extension` `Gemini API` `REST API`
> A Chrome extension that injects AI-generated reply controls directly into Gmail's compose UI, backed by a Spring Boot service.
- Built a Spring Boot REST backend that integrates the Gemini API to generate email replies conditioned on the original message content.
- Designed a mood-based generation system letting users select a tone (e.g. formal, casual, assertive) that is injected into the prompt to steer the generated reply's style.
- Built a Chrome extension using React components injected into the Gmail DOM to render reply-generation buttons directly within the existing compose window, avoiding a separate standalone UI.
- Structured the client-server integration around a stateless REST API, keeping the extension lightweight and the generation logic centralized on the backend.

### [Hybrid Lexical-Semantic Matching](https://github.com/shravan606756/hybrid-lexical-semantic-matching)
`Python` `NLP` `Scikit-learn` `Sentence Transformers` `Streamlit`
> An interpretable NLP pipeline for explainable candidate-role matching and deterministic skill-gap feedback.
- Built a multi-stage matching system combining TF-IDF-based lexical relevance scoring with MiniLM transformer embedding similarity.
- Designed a weighted linear aggregation model to balance keyword precision against contextual semantic similarity.
- Built an explainability layer that surfaces the top contributing sentences behind each ranking decision and generates deterministic, skill-gap-driven improvement feedback.
- Deployed the pipeline as an interactive Streamlit application for small-batch resume screening with visualized analytics.

<img src="https://capsule-render.vercel.app/api?type=rect&color=1a1a2e&height=2&section=header" width="100%"/>

## Technical Skills

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
      <img src="https://img.shields.io/badge/Embedding_Retrieval-1a1a2e?style=flat-square" />
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
