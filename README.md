<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=160&section=header&animation=twinkling" width="100%"/>

<a href="https://srikanthreddynandireddy.me"><img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=700&size=30&duration=3200&pause=900&color=A855F7&center=true&vCenter=true&width=900&height=60&lines=Hey!+%F0%9F%91%8B+I%27m+Srikanth+Reddy+Nandireddy;Applied+AI+%2F+LLM+Engineer;Agentic+Systems+%C2%B7+LLM+Evaluation+%C2%B7+RAG+%C2%B7+MLOps" alt="Hey! I'm Srikanth Reddy Nandireddy"/></a>

[![Portfolio](https://img.shields.io/badge/Portfolio-srikanthreddynandireddy.me-00d4ff?style=for-the-badge&logo=google-chrome&logoColor=white)](https://srikanthreddynandireddy.me)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/srikanth-reddy-nandireddy)
[![Kaggle](https://img.shields.io/badge/Kaggle-godvillain24-20BEFF?style=for-the-badge&logo=kaggle&logoColor=white)](https://www.kaggle.com/godvillain24)
[![Medium](https://img.shields.io/badge/Medium-Follow-12100E?style=for-the-badge&logo=medium&logoColor=white)](https://srikanth2314.medium.com/)
[![Email](https://img.shields.io/badge/Email-Hire%20Me-00e5a0?style=for-the-badge&logo=gmail&logoColor=white)](mailto:srikanthreddynandireddy@gmail.com)
[![Status](https://img.shields.io/badge/Status-Open%20to%20Work-00e5a0?style=for-the-badge&logoColor=white)](https://srikanthreddynandireddy.me#contact)

</div>

---

## 👋 About Me

```python
profile = {
    "name"         : "Srikanth Reddy Nandireddy",
    "role"         : "Applied AI / LLM Engineer",
    "education"    : "M.S. Data Science & AI — University of Central Missouri (May 2026)",
    "gpa"          : 4.0,
    "location"     : "United States",
    "open_to_work" : True,
    "available"    : "Immediately",
    "focus"        : ["Agentic Systems", "LLM Evaluation", "RAG", "Agent Safety", "MLOps"],
    "frameworks"   : ["LangGraph", "Microsoft Agent Framework", "MCP", "FastAPI", "Langfuse"],
    "latest"       : "Scholium — LangGraph research agent, live on Hugging Face Spaces",
    "hackathons"   : ["HackerRank Orchestrate Jun '26 — #16 / 1,773 (Top 1%)",
                      "HackerRank Orchestrate Aug '26 — #70 / 1,983"],
    "portfolio"    : "https://srikanthreddynandireddy.me",
    "gfg_streak"   : "255 consecutive days",
}
```

I build **agentic AI systems and the evaluation around them** — LangGraph agents with fail-closed
guardrails, frozen eval sets and regression gates, multi-agent Critic/Verifier loops, MCP
integrations, and the serving work that puts them behind a live endpoint you can hit with `curl`.
My READMEs publish where a system scores worse, not just where it scores best.

```bash
# Scholium is live — it answers from 150 arXiv ML papers and cites its sources.
# The Space sleeps when idle, so the first call can take a moment.
curl -s -X POST https://godvillain-scholium.hf.space/query -H 'Content-Type: application/json' -d '{"question": "What is the top-1 error rate achieved by LPA (mean + varied bound) using ResNet-110 on the CIFAR-100 dataset?", "stream": false}'
```

---

## 🚀 Featured Projects

<table>
<tr>
<td width="50%" valign="top">

### 📚 Scholium — LangGraph Research Agent &nbsp; [![Live](https://img.shields.io/badge/Live-Demo-00e5a0?style=flat-square&logo=huggingface&logoColor=white)](https://godvillain-scholium.hf.space)
Grounded QA agent over **150 arXiv ML papers** — my hand-rolled ReAct agent rebuilt as a typed **LangGraph** state graph with checkpoints and fail-closed guardrails. A **frozen 69-item eval set** drives a regression gate; the LLM judge is checked against 25 human-scored answers. Public **FastAPI** service on Hugging Face Spaces with SSE streaming, per-IP rate limiting, a restart-durable **$0.50/day cost ceiling**, and Langfuse tracing. Billing reconciliation showed only 24% of 27.27M billed prompt tokens had been recorded — the post-mortem publishes that, and where v3 scores *below* v2.1.

`LangGraph` `Gemini` `FastAPI` `Langfuse` `Docker` `HF Spaces`

[![GitHub](https://img.shields.io/badge/GitHub-View-181717?style=flat-square&logo=github)](https://github.com/GodVilan/langgraph-research-agent)
[![Post-mortem](https://img.shields.io/badge/Post--mortem-Read-6b7280?style=flat-square)](https://github.com/GodVilan/langgraph-research-agent/blob/main/docs/POSTMORTEM.md)

</td>
<td width="50%" valign="top">

### 🛰️ Multi-Modal Evidence Review
Two-stage **VLM agent** for insurance-claim adjudication — perception is split from reconciliation, so claim text and EXIF metadata cannot move a verdict. Ranked **16 / 1,773 — Top 1%** at HackerRank Orchestrate (June 2026). **95% valid-image accuracy** on 20 labeled claims (29 images), up from 60% single-pass; verdicts held on **7 of 8** adversarial injection twins; est. **~$0.017/claim** (44 claims, cold cache).

`Claude Sonnet 4.6` `VLM` `Prompt Engineering` `Eval-Driven Dev`

[![GitHub](https://img.shields.io/badge/GitHub-View-181717?style=flat-square&logo=github)](https://github.com/GodVilan/HackerRank-Orchestrate-June-2026)

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 📨 Message Notification Router
Personalized **notify / digest / mute** routing for **110 text, image, and voice messages**. *The model perceives, the code decides:* one Claude Sonnet 4.6 call returns a schema-forced reading, and a deterministic 4-layer precedence ladder sets the action, reason, and confidence. Ranked **#70 / 1,983** at HackerRank Orchestrate (August 2026). The eval report fixes its noise band before measuring and keeps the result that cut against the design: with the safety layers removed, accuracy was 27/30 vs. 25/30 — within noise.

`Claude Sonnet 4.6` `Vision` `faster-whisper` `Deterministic Rules` `Ablation`

[![GitHub](https://img.shields.io/badge/GitHub-View-181717?style=flat-square&logo=github)](https://github.com/GodVilan/Hackerrank-Orchestrate-aug26)
[![Eval Report](https://img.shields.io/badge/Eval%20Report-Read-6b7280?style=flat-square)](https://github.com/GodVilan/Hackerrank-Orchestrate-aug26/blob/HEAD/code/evaluation/evaluation_report.md)

</td>
<td width="50%" valign="top">

### 💊 MedsGuard Agent
LLM medication-logging agent with a **deterministic safety spine** — the model is load-bearing at exactly two edges, everything between is deterministic Python. Writes are gated by a **single-use signed JWT** (unique JTI, 300s TTL, subject binding), so a compromised model *provably* cannot log an off-schedule dose. A pass^k (k=5) harness surfaced 2 reflected injection leaks a single run missed.

`MCP` `Gemini 3.1 Pro` `HMAC + JWT` `SQLite` `HITL`

[![GitHub](https://img.shields.io/badge/GitHub-View-181717?style=flat-square&logo=github)](https://github.com/GodVilan/medsguard-agent)
[![Writeup](https://img.shields.io/badge/Writeup-Kaggle-20BEFF?style=flat-square&logo=kaggle&logoColor=white)](https://kaggle.com/competitions/vibecoding-agents-capstone-project/writeups/medsguard-an-llm-driven-medication-agent-with-a-d)

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🧠 TalentFabric AI
**5-agent** Microsoft Agent Framework system on Azure OpenAI and Microsoft Foundry — Planner-Executor plus a **Critic/Verifier loop-back** (capped at 2 iterations) that can flip *Not Ready → Ready* once it adds study hours. Hybrid BM25 + TF-IDF retrieval fused with a Microsoft Learn MCP client, all three Microsoft IQ layers, and an MLflow eval harness. Synthetic data only: 12 learners, 3 teams.

`Microsoft Agent Framework` `MCP` `Azure OpenAI` `RAG` `Streamlit`

[![GitHub](https://img.shields.io/badge/GitHub-View-181717?style=flat-square&logo=github)](https://github.com/GodVilan/TalentFabric-AI)
[![Demo](https://img.shields.io/badge/Demo-YouTube-FF0000?style=flat-square&logo=youtube&logoColor=white)](https://youtu.be/Vq-X2NIaruo)

</td>
<td width="50%" valign="top">

### 🛡️ Real-Time Fraud Detection (MLOps)
End-to-end MLOps system on **284,807 transactions** (0.172% fraud) — GitHub Actions CI/CD with a training workflow, **MLflow Model Registry** (PostgreSQL on Amazon RDS, artifacts in S3), and a Dockerized **FastAPI** service on AWS EC2 behind Nginx with `/predict` + `/predict-batch`, API-key auth, and rate limiting. SMOTE applied to the training split only.

`MLflow` `FastAPI` `Docker` `AWS` `GitHub Actions` `XGBoost`

[![GitHub](https://img.shields.io/badge/GitHub-View-181717?style=flat-square&logo=github)](https://github.com/GodVilan/Real-Time-CCFDS-With-MLOPs)

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🦠 US COVID-19 Mortality Forecasting &nbsp; [![Live](https://img.shields.io/badge/Live-Dashboard-00e5a0?style=flat-square&logo=render)](https://us-covid-19-mortality-intelligence.onrender.com/)
SARIMAX vs. Prophet vs. XGBoost on 3,300+ records with rolling cross-validation. Seasonal SARIMAX selected at **holdout MAE 138.14 vs. CV MAE 137.86**. 30-day forecasts with 95% confidence intervals in a Plotly Dash dashboard on Render.

`SARIMAX` `Prophet` `XGBoost` `Plotly Dash` `Docker`

[![GitHub](https://img.shields.io/badge/GitHub-View-181717?style=flat-square&logo=github)](https://github.com/GodVilan/US-COVID-19-Mortality-Intelligence-Forecasting-System)

</td>
<td width="50%" valign="top">

### 🎭 Multimodal Emotion Recognition
BERT + Wav2Vec2 + ViT cross-modal **Transformer fusion** (4 layers, 8 heads). **59.96% accuracy, 60.66% weighted F1** on 7-class MELD, with class-weighted loss for label imbalance.

`PyTorch` `BERT` `Wav2Vec2` `ViT` `HuggingFace`

[![GitHub](https://img.shields.io/badge/GitHub-View-181717?style=flat-square&logo=github)](https://github.com/GodVilan/Multimodal-Emotion-Recognition-MELD-via-Cross-Modal-Transformers)

</td>
</tr>
</table>

**Also on the bench**

- 🔍 [arXiv Agent v2.1](https://github.com/GodVilan/arXiv-Agent) — Scholium's predecessor: hand-rolled ReAct loop, layout-aware RAG, adversarial peer-review audit, recursive citation tracing
- 📊 [arXiv RAG Benchmark](https://github.com/GodVilan/arXiv-rag) — empirical study of 4 retrievers × 3 chunk sizes over 150 papers
- 🎬 [DARE-Rec](https://github.com/GodVilan/Netflix-Personalized-Recommender) — LightGCN + EASE^R + iALS ensemble with MMR diversity re-ranking and a Thompson Sampling bandit (simulated A/B), served with FastAPI + Docker
- 📰 [Fake News Detection](https://github.com/GodVilan/Fake-News-Detection-Using-TF-IDF-Logistic-Regression-and-DistilBERT-Transformer-Models) — TF-IDF + Logistic Regression vs. DistilBERT on 62,834 articles, with F1-threshold tuning

---

## 🛠️ Tech Stack

<div align="center">

**Languages**

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=postgresql&logoColor=white)
![R](https://img.shields.io/badge/R-276DC3?style=flat-square&logo=r&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white)
![Bash](https://img.shields.io/badge/Bash-4EAA25?style=flat-square&logo=gnubash&logoColor=white)

**Agents & LLM Systems**

![LangGraph](https://img.shields.io/badge/LangGraph-1C3C3C?style=flat-square&logoColor=white)
![Microsoft Agent Framework](https://img.shields.io/badge/Microsoft%20Agent%20Framework-0078D4?style=flat-square&logo=microsoft&logoColor=white)
![MCP](https://img.shields.io/badge/MCP-5C2D91?style=flat-square&logoColor=white)
![ReAct](https://img.shields.io/badge/ReAct%20Agents-a855f7?style=flat-square&logoColor=white)
![RAG](https://img.shields.io/badge/RAG%20Pipelines-00d4ff?style=flat-square&logoColor=white)
![FAISS](https://img.shields.io/badge/FAISS-0078D4?style=flat-square&logoColor=white)
![Claude API](https://img.shields.io/badge/Claude%20API-D97757?style=flat-square&logo=anthropic&logoColor=white)
![Gemini API](https://img.shields.io/badge/Gemini%20API-4285F4?style=flat-square&logo=googlegemini&logoColor=white)

**LLM Evaluation & Observability**

![Langfuse](https://img.shields.io/badge/Langfuse-0A0A0A?style=flat-square&logoColor=white)
![Eval Sets](https://img.shields.io/badge/Frozen%20Eval%20Sets-6b7280?style=flat-square&logoColor=white)
![Regression Gates](https://img.shields.io/badge/Regression%20Gates-6b7280?style=flat-square&logoColor=white)
![pass^k](https://img.shields.io/badge/pass%5Ek%20Harnesses-6b7280?style=flat-square&logoColor=white)
![LLM-as-Judge](https://img.shields.io/badge/LLM--as--Judge-6b7280?style=flat-square&logoColor=white)

**ML & Deep Learning**

![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=flat-square&logo=tensorflow&logoColor=white)
![HuggingFace](https://img.shields.io/badge/HuggingFace-FFD21E?style=flat-square&logo=huggingface&logoColor=black)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-F7931E?style=flat-square&logo=scikit-learn&logoColor=white)
![XGBoost](https://img.shields.io/badge/XGBoost-FF6600?style=flat-square&logoColor=white)

**Cloud & MLOps**

![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonaws&logoColor=white)
![Azure OpenAI](https://img.shields.io/badge/Azure%20OpenAI-0078D4?style=flat-square&logo=microsoftazure&logoColor=white)
![MLflow](https://img.shields.io/badge/MLflow-0194E2?style=flat-square&logo=mlflow&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![Hugging Face Spaces](https://img.shields.io/badge/HF%20Spaces-FFD21E?style=flat-square&logo=huggingface&logoColor=black)

</div>

---

## 📊 GitHub Stats

<div align="center">

<img height="160" src="https://github-readme-stats.vercel.app/api?username=GodVilan&show_icons=true&theme=tokyonight&hide_border=true&bg_color=030912&title_color=00d4ff&icon_color=00e5a0&text_color=ddeeff&count_private=true" />
<img height="160" src="https://github-readme-stats.vercel.app/api/top-langs/?username=GodVilan&layout=compact&theme=tokyonight&hide_border=true&bg_color=030912&title_color=00d4ff&text_color=ddeeff&langs_count=6" />

</div>

<div align="center">

[![GitHub Streak](https://streak-stats.demolab.com?user=GodVilan&theme=tokyonight&hide_border=true&background=030912&stroke=00d4ff&ring=00e5a0&fire=a855f7&currStreakLabel=00d4ff&sideLabels=ddeeff&dates=6b85a3)](https://github.com/GodVilan)

</div>

<div align="center">

<img width="98%" src="https://github-readme-activity-graph.vercel.app/graph?username=GodVilan&bg_color=030912&color=ddeeff&line=a855f7&point=00e5a0&area=true&area_color=00d4ff&title_color=00d4ff&hide_border=true&custom_title=Contribution%20Graph" />

</div>

---

## 🏆 Honors & Achievements

| Award | Details |
|---|---|
| 🥇 **Graduate Student Achievement Award 2025–2026** | University of Central Missouri Graduate Studies — *Recognized for exceptional scholastic achievement, exemplary contributions to Data Science & AI, and outstanding character and leadership* |
| 🏅 **HackerRank Orchestrate — Top 1%** | Ranked **16 / 1,773** · 24-hour AI agent hackathon (June 2026) |
| 🎖️ **HackerRank Orchestrate — August 2026** | Ranked **70 / 1,983** · Final score 73.1 / 100 (up from 66.5 in June) |
| 🥇 **Global Rank 1** | CodeChef May Long Two — Division 4 Rated |
| 🏆 **National Finalist** | IICC Coding Competition — Top 1% of 100,000+ participants |
| 🥉 **Bronze Medal** | Ranked Top 3 in B.Tech Academic Program |
| ⭐ **5★ HackerRank** | Data Structures & Algorithms |
| 🔥 **255-Day Streak** | GeeksforGeeks Problem of the Day |

---

## 🎓 Education & Certifications

| Degree | Institution | GPA |
|---|---|---|
| **M.S. Data Science & AI** *(2024–2026)* | University of Central Missouri | **4.0 / 4.0** |
| **B.Tech CSE (Hons.)** *(2020–2024)* | CMR College of Engineering & Technology | **9.06 / 10.0** |

**Certifications:** Microsoft Applied Skills — Get started developing agents in Microsoft Foundry · Anthropic — Introduction to Model Context Protocol · Anthropic — AI Fluency: Framework & Foundations · AWS Academy Graduate — Data Analytics & Cloud Foundations · Google — Foundations: Data, Data, Everywhere (Google Data Analytics Certificate)

---

## 🎖️ Verified Badges

<!--START_SECTION:badges-->
[![AI Skills Fest 2026](https://images.credly.com/size/80x80/images/082c8d0c-5232-4597-b6c4-6bebcc4f3046/blob)](https://www.credly.com/badges/775304f3-1c70-41c2-b7cb-a4d9f0d92406)
[![AWS Academy Graduate - AWS Academy Data Analytics](https://images.credly.com/size/80x80/images/4a489a8c-0b2d-40ee-a839-afa55b44208d/image.png)](https://www.credly.com/badges/2d5d029b-ac6b-48df-9420-170649c50729)
[![AWS Academy Graduate - Cloud Foundations - Training Badge](https://images.credly.com/size/80x80/images/e3541a0c-dd4a-4820-8052-5001006efc85/blob)](https://www.credly.com/badges/00efbea6-a4ef-4016-87ed-23f91335b94b)
<!--END_SECTION:badges-->

---

## 📬 Let's Connect

<div align="center">

I'm actively seeking **full-time Applied AI / LLM Engineer & ML Engineer roles** in the **United States** — available immediately.

[![Portfolio](https://img.shields.io/badge/🌐%20Portfolio-srikanthreddynandireddy.me-00d4ff?style=for-the-badge)](https://srikanthreddynandireddy.me)
[![LinkedIn](https://img.shields.io/badge/💼%20LinkedIn-Connect-0077B5?style=for-the-badge)](https://www.linkedin.com/in/srikanth-reddy-nandireddy)
[![Kaggle](https://img.shields.io/badge/📊%20Kaggle-godvillain24-20BEFF?style=for-the-badge)](https://www.kaggle.com/godvillain24)
[![Medium](https://img.shields.io/badge/✍️%20Medium-Read%20Articles-12100E?style=for-the-badge&logo=medium&logoColor=white)](https://srikanth2314.medium.com/)
[![Email](https://img.shields.io/badge/✉️%20Email-srikanthreddynandireddy@gmail.com-00e5a0?style=for-the-badge)](mailto:srikanthreddynandireddy@gmail.com)

</div>

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=100&section=footer" width="100%"/>
