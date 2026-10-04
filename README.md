<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:7a2e2a,100:8a6a1f&height=190&section=header&text=Bernice%20Malaiarasu&fontSize=48&fontColor=faf8f3&fontAlignY=36&desc=Generative%20AI%20Engineer%20%C2%B7%20MS%20AI%20%40%20Northeastern&descSize=18&descAlignY=58&descAlign=50" alt="Bernice Malaiarasu, Generative AI Engineer" width="100%" />
</p>

<p align="center">
  <a href="https://bernice511.github.io">
    <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=20&duration=3000&pause=900&color=7A2E2A&center=true&vCenter=true&width=560&lines=Building+production+multi-agent+systems;RAG+%C2%B7+Text-to-SQL+%C2%B7+LLM+evals;Bayer+GenAI+Award+winner;Open+to+Spring+2027+Agentic+AI+internships" alt="Building production multi-agent systems · RAG · Text-to-SQL · LLM evals · Open to Spring 2027 Agentic AI internships" />
  </a>
</p>

<p align="center">
  <a href="https://bernice511.github.io"><img src="https://img.shields.io/badge/Portfolio-7a2e2a?style=for-the-badge&logo=googlechrome&logoColor=white" alt="Portfolio" /></a>
  <a href="https://linkedin.com/in/bernice-mercy"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
  <a href="mailto:bernicemalaiarasu@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" /></a>
</p>

I build production LLM systems that people actually use. I have 4+ years in software and data engineering, including 2+ years shipping multi-agent GenAI at **Thoughtworks** for Bayer, where RAG, Text-to-SQL and NER run against **18,000+ preclinical safety studies**. I'm now doing an MS in AI (ML specialization) at Northeastern's **Khoury College** and working as a Research Assistant at the **AIMES Lab**.

> 🔍 **Open to Spring 2027 Agentic AI internships.** See my [portfolio](https://bernice511.github.io) or [reach out](mailto:bernicemalaiarasu@gmail.com).

## 🔭 What I'm Working On
- 📰 **[NewsroomFeed](https://newsroomfeed.duckdns.org/)** (AIMES Lab): a LangGraph pipeline that turns live civic feeds (MassDOT, NWS, Boston 311) into hyperlocal AI news. A journalist approves every item before it publishes. Shipped as a Next.js PWA.
- 🎓 **Husky AI** (AIMES Lab): a platform where students practice prompt engineering through interactive exercises and guided feedback.

## 🧪 Selected Projects
| Project | What it does | Highlight |
|---|---|---|
| [**Entiscribe**](https://github.com/bernice511/entiscribe) | Extracts user-defined entities from PDFs with an LLM, evaluates the extraction, and links entities into a knowledge graph | LangGraph · runs fully local, no API keys |
| [**Crisis-Aware Dialogue**](https://github.com/bernice511/crisis-aware-dialogue) | Routes distress-signal input with a RoBERTa classifier into a QLoRA-fine-tuned Llama-3.2-1B | 0.920 F1 at ~1/100th of GPT-5's size |
| [**Delivery Delay Prediction**](https://github.com/bernice511/delivery_prediction) | Two-stage XGBoost that flags late Olist orders before they ship, with a SHAP-explained Streamlit dashboard | 0.922 ROC-AUC on 100K+ orders |
| [**Job Applier**](https://github.com/bernice511/jobApplier) | Tailors resumes and cover letters to real JDs, with guardrails against fabrication | Human-in-the-loop, never auto-submits |

## 🚀 Featured: PRINCE @ Thoughtworks for Bayer
**PRINCE (Preclinical Information Centre)** is a supervisor-orchestrated multi-agent knowledge engine used in Bayer's daily preclinical drug-safety research. I worked on it from 2022 to 2025, first on its data platform and then leading development of the GenAI system. It won the 🏆 **Bayer GenAI Award for Best Technical Implementation** (2025).

```mermaid
flowchart LR
    Q([Researcher question]) --> S{{Supervisor agent}}
    S --> R[Researcher agent]
    S --> F[Reflection agent]
    S --> P[Document planner]
    S --> W[Writer agent]
    R --> RAG[(Hybrid RAG<br/>OpenSearch + reranker)]
    R --> SQL[(Text-to-SQL<br/>AWS Athena)]
    F -. needs more evidence .-> R
    W --> H[/Human review/]
    H --> A([Citation-linked answer])
```

| | |
|---|---|
| 🔎 **Hybrid RAG** | 0.7 vector / 0.3 keyword search over 100 GB+ of biomedical data, re-ranked with bge-reranker |
| 🧮 **Text-to-SQL** | Dynamic few-shot prompting against AWS Athena, **90%+ accuracy** |
| 🏷️ **NER extraction** | Metadata pulled from study reports, **98%+ accuracy across 40+ fields** |
| ✅ **Eval as a CI gate** | RAGAS + DeepEval on every change, with Langfuse tracing |
| 📈 **Impact** | Ad-hoc data requests went from days to minutes, and complex queries got 30% faster |

## 🛠 Tech Stack
**GenAI**<br/>
<img src="https://img.shields.io/badge/LangGraph-1C3C3C?style=flat-square&logo=langchain&logoColor=white" alt="LangGraph" /> <img src="https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white" alt="LangChain" /> <img src="https://img.shields.io/badge/CrewAI-FF5A50?style=flat-square" alt="CrewAI" /> <img src="https://img.shields.io/badge/RAG-7a2e2a?style=flat-square" alt="RAG" /> <img src="https://img.shields.io/badge/Langfuse-0A0A0A?style=flat-square" alt="Langfuse" /> <img src="https://img.shields.io/badge/RAGAS-6A1B9A?style=flat-square" alt="RAGAS" /> <img src="https://img.shields.io/badge/DeepEval-6A1B9A?style=flat-square" alt="DeepEval" /> <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white" alt="PyTorch" /> <img src="https://img.shields.io/badge/HuggingFace-FFD21E?style=flat-square&logo=huggingface&logoColor=black" alt="HuggingFace" />

**Languages & Frameworks**<br/>
<img src="https://img.shields.io/badge/Python-3670A0?style=flat-square&logo=python&logoColor=ffdd54" alt="Python" /> <img src="https://img.shields.io/badge/TypeScript-007ACC?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript" /> <img src="https://img.shields.io/badge/Scala-DE3226?style=flat-square&logo=scala&logoColor=white" alt="Scala" /> <img src="https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white" alt="Java" /> <img src="https://img.shields.io/badge/Kotlin-7F52FF?style=flat-square&logo=kotlin&logoColor=white" alt="Kotlin" /> <img src="https://img.shields.io/badge/SQL-00758F?style=flat-square&logo=mysql&logoColor=white" alt="SQL" /> <img src="https://img.shields.io/badge/FastAPI-005571?style=flat-square&logo=fastapi" alt="FastAPI" /> <img src="https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=next.js&logoColor=white" alt="Next.js" /> <img src="https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white" alt="Streamlit" />

**Cloud & Data**<br/>
<img src="https://img.shields.io/badge/AWS-FF9900?style=flat-square&logo=amazonwebservices&logoColor=white" alt="AWS" /> <img src="https://img.shields.io/badge/OpenSearch-005EB8?style=flat-square&logo=opensearch&logoColor=white" alt="OpenSearch" /> <img src="https://img.shields.io/badge/Elasticsearch-005571?style=flat-square&logo=elasticsearch&logoColor=white" alt="Elasticsearch" /> <img src="https://img.shields.io/badge/Apache_Spark-E25A1C?style=flat-square&logo=apachespark&logoColor=white" alt="Apache Spark" /> <img src="https://img.shields.io/badge/AWS_Glue-8C4FFF?style=flat-square" alt="AWS Glue" /> <img src="https://img.shields.io/badge/Step_Functions-E7157B?style=flat-square" alt="Step Functions" /> <img src="https://img.shields.io/badge/Terraform-5835CC?style=flat-square&logo=terraform&logoColor=white" alt="Terraform" /> <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" alt="Docker" /> <img src="https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white" alt="GitHub Actions" />

<details>
<summary><b>🎤 Speaking & Mentorship</b></summary>
<br/>

- **XConf, Thoughtworks Bangalore (Aug 2025):** PRINCE's multi-agent architecture and LLM evaluation strategies
- **GenAI Workshop Facilitator (Mar 2025):** designed and delivered a hands-on LLM & RAG workshop for 50+ developers
- **GeekNight (Dec 2024):** improving Text-to-SQL accuracy with dynamic few-shot prompting, for 80+ engineers

</details>

<details>
<summary><b>📚 Writing & Recognition</b></summary>
<br/>

- 📝 **[From Unstructured to Structured: Adobe PDF Extract API for Data Transformation](https://dev.to/theblogsquad/from-unstructured-to-structured-adobe-pdf-extract-api-for-data-transformation-1n08)** on *Dev.to*: a practical guide to turning messy PDF data into clean, usable formats.
- 📄 **Frontiers in Artificial Intelligence (2025):** PRINCE is described in the peer-reviewed paper *[From data silos to insights: the PRINCE multi-agent knowledge engine for preclinical drug development](https://doi.org/10.3389/frai.2025.1636809)*, which acknowledges my contributions as part of the Thoughtworks team.

</details>

## 💬 Ask me about
Building multi-agent systems, LLM evaluation, the move from Chennai to Boston, or my dream of building a RAG-based search engine for my fictional book multiverse.

## 📊 GitHub Stats
<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=bernice511&show_icons=true&hide_border=true&include_all_commits=true&count_private=true&bg_color=faf8f3&title_color=7a2e2a&text_color=16150f&icon_color=8a6a1f" alt="Bernice's GitHub Stats" height="170px" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=bernice511&layout=compact&hide_border=true&langs_count=6&bg_color=faf8f3&title_color=7a2e2a&text_color=16150f" alt="Top Languages" height="170px" />
</p>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:8a6a1f,100:7a2e2a&height=90&section=footer" width="100%" alt="" />
