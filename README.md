<div align="center">

<!-- Animated Typing Banner -->
[![Typing SVG](https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=700&size=28&duration=3000&pause=800&color=6C63FF&center=true&vCenter=true&multiline=true&repeat=true&width=800&height=100&lines=Durgam+Poojitha;AI+Engineer+%7C+Computer+Vision+%7C+LLM+Systems)](https://git.io/typing-svg)

**`Architecting Intelligent Systems · Medical AI · Foundation Models · Production ML`**

<br/>

[![Portfolio](https://img.shields.io/badge/Portfolio-000000?style=for-the-badge&logo=vercel&logoColor=white)](https://portfolio-woad-mu-53.vercel.app/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/poojitha-durgam-856a0b291)
[![Email](https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:durgampoojitha19@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/poojithadurgam)

<br/>

![Profile Views](https://komarev.com/ghpvc/?username=poojithadurgam&color=6C63FF&style=for-the-badge&label=PROFILE+VIEWS)

</div>

---

## ⚡ Engineering AI Systems at Scale

```python
class AIEngineer:
    name       = "Durgam Poojitha"
    education  = "B.Tech CSE · Amrita School of Engineering · 2023–2027"
    focus      = ["Medical AI", "Computer Vision", "LLM Systems", "Agentic AI"]
    current    = "Agentic nucleus segmentation with SAM + foundation models on PanNuke"
    building   = ["RAG pipelines", "Multi-agent systems", "End-to-end ML platforms"]
    looking_for = ["AI/ML Engineering Internships", "Research Internships", "SWE Roles"]
```

Engineering AI systems that transform raw data into production-grade intelligence. Experienced in designing end-to-end machine learning pipelines — from data ingestion and model experimentation to deployment and monitoring. Specializing in Computer Vision, Medical Imaging, and LLM-powered applications with a strong foundation in scalable backend architecture.

Currently conducting research on agentic segmentation pipelines using Segment Anything Models (SAM ViT-B) applied to histopathology, iteratively engineering uncertainty-guided correction modules that push beyond baseline segmentation accuracy on real clinical imaging data.

---

## 🏗️ What I Build

<table>
<tr>
<td width="50%" valign="top">

**🧠 AI-Powered Systems**
- Agentic pipelines with multi-step reasoning and self-correction
- RAG systems grounding LLMs in domain-specific knowledge
- Multi-agent orchestration for automated research workflows
- Foundation model fine-tuning and inference optimization

</td>
<td width="50%" valign="top">

**👁️ Computer Vision**
- Medical image segmentation with SAM and ViT backbones
- Instance and semantic segmentation on clinical datasets
- Uncertainty-aware inference for safety-critical applications
- Vision-language model integrations

</td>
</tr>
<tr>
<td width="50%" valign="top">

**⚙️ Backend & Platform Engineering**
- Distributed FastAPI services with WebSocket streaming
- Microservice architectures containerized with Docker
- Vector databases (ChromaDB) for semantic retrieval
- RESTful and real-time APIs built for production scale

</td>
<td width="50%" valign="top">

**📊 Data Intelligence**
- End-to-end ML pipelines from raw data to serving
- Business intelligence dashboards with real-time analytics
- Feature engineering systems for structured and unstructured data
- Automated model evaluation and drift monitoring

</td>
</tr>
</table>

---

## 🚀 Featured Projects

<details>
<summary><b>🔬 01 · Agentic Medical Imaging Platform (SAM + UICE Pipeline)</b></summary>
<br/>

**Problem:** Automated nucleus segmentation in H&E histopathology images is brittle under standard thresholding — existing baselines fail to generalize across cell morphologies in clinical datasets.

**Architecture:** Uncertainty-Guided Iterative Correction Engine (UICE) layered on SAM ViT-B. N1 generates candidate masks, N2 applies uncertainty estimation via boundary-ring thresholding, N6 performs iterative mask correction based on confidence scoring. Multi-scale aggregation (MSA) as the evaluation protocol.

**Tech Stack:** `Python` · `PyTorch` · `SAM ViT-B` · `PanNuke Dataset` · `Jupyter` · `NumPy` · `OpenCV`

**Engineering Impact:**
- Improved MSA from ~0.147 AMG baseline to ~0.46 with the full agentic correction pipeline
- Replaced brittle hard-threshold uncertainty with relative boundary-ring scoring for robustness
- Designed module ordering (N1→N2→N6) resolving architectural sequencing bugs in prior implementations

**What Recruiters Should Notice:** Production mindset applied to research — identifying and resolving root-cause architectural bugs, quantifying improvements at each pipeline stage, and grounding design decisions in clinical imaging constraints.

---
</details>

<details>
<summary><b>🤖 02 · AgentIQ — Multi-Agent Research & Coding Assistant</b></summary>
<br/>

**Problem:** Developers and researchers lose hours context-switching between code generation, documentation lookup, and synthesis tasks — with no unified intelligent workspace.

**Architecture:** Six specialized autonomous agents (Planner, Researcher, Coder, Reviewer, Synthesizer, Memory) coordinated via a FastAPI orchestration layer. Real-time responses streamed over WebSockets. ChromaDB vector memory enables persistent context across sessions.

**Tech Stack:** `Python` · `FastAPI` · `WebSockets` · `ChromaDB` · `React` · `TypeScript` · `Docker` · `LangChain`

**Engineering Impact:**
- Sub-200ms agent handoff latency via async task queuing
- Persistent semantic memory reducing redundant LLM calls by ~40%
- Modular agent architecture supports hot-swapping individual agents without system restart

**What Recruiters Should Notice:** Full-stack multi-agent system engineered from scratch — not a tutorial wrapper. Demonstrates systems thinking, async architecture design, and production engineering discipline.

---
</details>

<details>
<summary><b>🏥 03 · Healthcare RAG Copilot</b></summary>
<br/>

**Problem:** Clinical professionals and researchers waste critical time parsing dense medical literature. Generic LLMs hallucinate on domain-specific queries.

**Architecture:** Retrieval-Augmented Generation pipeline ingesting medical documents via semantic chunking → embeddings stored in a vector index → top-k retrieval grounding GPT-4 responses with cited sources. Custom re-ranking layer filters for clinical relevance before generation.

**Tech Stack:** `Python` · `FastAPI` · `LangChain` · `ChromaDB` · `OpenAI API` · `React` · `PostgreSQL`

**Engineering Impact:**
- Reduced hallucination rate vs. vanilla LLM baseline via grounded retrieval
- Achieved sub-2s end-to-end query-to-cited-response latency
- Multi-document cross-referencing with traceable source attribution per claim

**What Recruiters Should Notice:** Domain-specific AI system built with a clinical safety mindset — prioritizing verifiability and hallucination mitigation over raw fluency.

---
</details>

<details>
<summary><b>📊 04 · Real-Time Business Intelligence Platform</b></summary>
<br/>

**Problem:** Mid-sized businesses operate on delayed batch reports — missing real-time signals that drive revenue decisions.

**Architecture:** Event-driven data ingestion pipeline → streaming aggregations → FastAPI analytics backend → React dashboard with WebSocket-pushed updates. PostgreSQL for persistent storage with pre-computed materialized views for sub-100ms dashboard loads.

**Tech Stack:** `Python` · `FastAPI` · `PostgreSQL` · `React` · `TypeScript` · `WebSockets` · `Docker` · `Tailwind CSS`

**Engineering Impact:**
- Real-time KPI updates with <100ms dashboard refresh latency
- Configurable alert engine triggering on threshold anomalies
- Role-based access control with multi-tenant data isolation

**What Recruiters Should Notice:** Full-stack engineering with production data patterns — streaming architecture, materialized views, and real-time UX without sacrificing query correctness.

---
</details>

<details>
<summary><b>🎯 05 · AI Interview Coach</b></summary>
<br/>

**Problem:** Interview preparation is fragmented — candidates have no adaptive system that simulates real interviews, tracks weaknesses, and generates targeted practice.

**Architecture:** LLM-powered question generation calibrated to role/level → speech-to-text transcription of candidate responses → structured rubric-based evaluation → personalized improvement plan generation. Progress tracked per topic in PostgreSQL.

**Tech Stack:** `Python` · `FastAPI` · `OpenAI API` · `React` · `TypeScript` · `PostgreSQL` · `Whisper API`

**Engineering Impact:**
- Adaptive question difficulty based on response quality scoring
- Structured evaluation across 6 dimensions: correctness, communication, depth, examples, structure, confidence
- Personalized study plan generated from longitudinal performance data

**What Recruiters Should Notice:** Closed-loop AI product — ingests, evaluates, and improves. Demonstrates product thinking alongside engineering execution.

---
</details>

<details>
<summary><b>⚡ 06 · Distributed Recommendation Engine</b></summary>
<br/>

**Problem:** Static recommendation systems degrade under catalog scale and fail to capture evolving user preferences in real-time.

**Architecture:** Hybrid collaborative + content-based filtering. User interaction events processed via async workers → embedding updates in near-real-time → top-N retrieval from vector index → Spring Boot serving layer with response caching.

**Tech Stack:** `Java` · `Spring Boot` · `Python` · `PostgreSQL` · `MongoDB` · `Docker` · `Go`

**Engineering Impact:**
- Horizontal scaling design supporting 10k+ concurrent recommendation requests
- Cold-start handling via content-based fallback for new users/items
- A/B testing instrumentation built into serving layer

**What Recruiters Should Notice:** Systems-level thinking at scale — distributed design patterns, hybrid modeling strategy, and production serving architecture.

---
</details>

---

## 🧠 AI & Machine Learning Expertise

<div align="center">

| Domain | Capabilities |
|--------|-------------|
| **Foundation Models** | SAM, ViT, GPT-4, fine-tuning, prompt engineering, adapter layers |
| **Computer Vision** | Segmentation, detection, medical imaging, uncertainty estimation |
| **Generative AI** | LLM applications, RAG systems, multi-modal pipelines |
| **Agentic AI** | Multi-agent orchestration, tool-use, iterative correction loops |
| **NLP** | Text classification, semantic search, embeddings, summarization |
| **MLOps** | Pipeline automation, model evaluation, experiment tracking |

</div>

---

## 🛠️ Tech Stack

<div align="center">

**Languages**

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=cplusplus&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Go](https://img.shields.io/badge/Go-00ADD8?style=for-the-badge&logo=go&logoColor=white)
![Haskell](https://img.shields.io/badge/Haskell-5D4F85?style=for-the-badge&logo=haskell&logoColor=white)

**Frontend**

![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Angular](https://img.shields.io/badge/Angular-DD0031?style=for-the-badge&logo=angular&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)

**Backend**

![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=node.js&logoColor=white)
![Express.js](https://img.shields.io/badge/Express.js-000000?style=for-the-badge&logo=express&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=for-the-badge&logo=spring-boot&logoColor=white)

**Databases**

![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![ChromaDB](https://img.shields.io/badge/ChromaDB-FF6B35?style=for-the-badge&logo=databricks&logoColor=white)

**AI / ML**

![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=for-the-badge&logo=opencv&logoColor=white)
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=for-the-badge&logo=langchain&logoColor=white)
![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=for-the-badge&logo=openai&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)

**DevOps & Tools**

![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![Postman](https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=postman&logoColor=white)

</div>

---

## 🎯 Engineering Focus Areas

<table>
<tr>
<td width="33%" valign="top">

**🧠 AI Engineering**
Designing end-to-end ML pipelines from raw data ingestion to model serving. Emphasis on uncertainty quantification, iterative correction, and evaluation rigor — not just benchmarks.

</td>
<td width="33%" valign="top">

**👁️ Computer Vision**
Engineered segmentation systems on clinical imaging data using SAM-based foundation models. Experienced in instance segmentation, uncertainty estimation, and multi-scale aggregation.

</td>
<td width="33%" valign="top">

**🔮 Generative AI**
Building LLM-powered applications grounded in retrieval-augmented generation. Focused on hallucination mitigation, source attribution, and production reliability.

</td>
</tr>
<tr>
<td width="33%" valign="top">

**⚙️ Backend Systems**
Architecting scalable APIs with FastAPI, Spring Boot, and Node.js. Experienced in WebSocket-based real-time systems, async task queues, and microservice decomposition.

</td>
<td width="33%" valign="top">

**📊 Data Engineering**
Designing feature engineering pipelines, streaming aggregation systems, and analytics backends. Emphasis on correctness, latency, and maintainability at scale.

</td>
<td width="33%" valign="top">

**🤖 Agentic Systems**
Orchestrating autonomous multi-agent pipelines with tool use, memory, and iterative self-correction. Designing agent handoff protocols that hold up under adversarial inputs.

</td>
</tr>
</table>

---

## 🔬 Research Interests

```
Foundation Models  ·  Medical Image Segmentation  ·  Vision Transformers
Multimodal AI  ·  Agentic Pipelines  ·  Uncertainty-Aware Inference
Histopathology AI  ·  Segment Anything Models  ·  Healthcare AI
```

Investigating how foundation models can be adapted for safety-critical medical imaging tasks with minimal labeled data. Current focus: agentic correction pipelines that iteratively refine segmentation outputs using boundary uncertainty signals — moving beyond one-shot inference toward systems that reason about their own confidence.

Long-term research trajectory: building AI systems for healthcare that are not only accurate but interpretable, uncertainty-aware, and deployable in real clinical environments.

---

## 🔧 Currently Building

<div align="center">

```
┌─────────────────────────────────────────────────────────────────┐
│                  ACTIVE ENGINEERING FOCUS                       │
├─────────────────────────────────────────────────────────────────┤
│  🔬  SAM-based Agentic Nucleus Segmentation (UICE Pipeline)    │
│  🤖  Multi-Agent LLM Orchestration Systems                      │
│  📚  RAG Pipelines for Domain-Specific AI Applications          │
│  🧪  Uncertainty Quantification in Medical Vision Models        │
│  ⚡  End-to-End ML Pipelines with Automated Evaluation          │
└─────────────────────────────────────────────────────────────────┘
```

</div>

---

## 📈 GitHub Analytics

<div align="center">

<img height="180em" src="https://github-readme-stats.vercel.app/api?username=poojithadurgam&show_icons=true&theme=tokyonight&include_all_commits=true&count_private=true&hide_border=true&bg_color=0D1117&title_color=6C63FF&icon_color=6C63FF&text_color=FFFFFF"/>
<img height="180em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=poojithadurgam&layout=compact&langs_count=8&theme=tokyonight&hide_border=true&bg_color=0D1117&title_color=6C63FF&text_color=FFFFFF"/>

</div>

<div align="center">

<img src="https://github-readme-streak-stats.herokuapp.com/?user=poojithadurgam&theme=tokyonight&hide_border=true&background=0D1117&stroke=6C63FF&ring=6C63FF&fire=FF6B6B&currStreakLabel=6C63FF"/>

</div>

<div align="center">

[![Poojitha's Activity Graph](https://github-readme-activity-graph.vercel.app/graph?username=poojithadurgam&bg_color=0D1117&color=6C63FF&line=6C63FF&point=FFFFFF&area=true&hide_border=true)](https://github.com/ashutosh00710/github-readme-activity-graph)

</div>

---

## 🏆 Engineering Philosophy

<table>
<tr>
<td width="25%" align="center">

**🔍 Systems Thinking**
Every component designed with the full pipeline in mind — from data to deployment to failure modes.

</td>
<td width="25%" align="center">

**📐 Research Rigor**
Quantified evaluation at each stage. No improvements claimed without measurement.

</td>
<td width="25%" align="center">

**🛠️ Production Mindset**
Code architected for readability, extensibility, and production reliability — not just passing tests.

</td>
<td width="25%" align="center">

**📈 Continuous Iteration**
Systems improved through systematic debugging, ablation, and root-cause analysis.

</td>
</tr>
</table>

---

## 🤝 Open to Collaboration

Actively seeking collaborations on:

- 🔬 **AI / ML Research** — Medical imaging, segmentation, foundation model applications
- 🤖 **Agentic Systems** — Multi-agent pipelines, LLM tool use, autonomous workflows  
- 🧬 **Healthcare AI** — Clinical NLP, imaging AI, patient-facing AI products
- 🚀 **Startup Projects** — Building from 0→1 on AI-native products
- 📖 **Open Source AI** — Contributing to meaningful ML tooling and research repos

If you're building something ambitious in AI, reach out.

---

## 📬 Get in Touch

<div align="center">

| Platform | Link |
|----------|------|
| 🌐 Portfolio | [portfolio-woad-mu-53.vercel.app](https://portfolio-woad-mu-53.vercel.app/) |
| 💼 LinkedIn | [poojitha-durgam-856a0b291](https://www.linkedin.com/in/poojitha-durgam-856a0b291) |
| 📧 Email | [durgampoojitha19@gmail.com](mailto:durgampoojitha19@gmail.com) |
| 🐙 GitHub | [@poojithadurgam](https://github.com/poojithadurgam) |

</div>

---

<div align="center">

*Engineered with intent. Built to ship.*

</div>
