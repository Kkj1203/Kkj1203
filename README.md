# Hi there 👋 I'm Keerthikrishna Jog

🧠 **AI Engineer | Machine Learning | LLMs | MLOps**  
💼 AI Engineer at **Zensar Technologies**, working for a **Fortune 500 insurance client**  
📍 Pune, India (Remote)  
🎓 B.Tech in Computer Science (AI & Analytics), MIT ADT University · CGPA 8.9

I build machine-learning and LLM systems and take them all the way to production: from cleaning raw data and designing models to Kubernetes deployment, automated retraining and monitoring. I care about honest evaluation: measuring what really works, including when a simpler ML model beats an LLM.

---

## 💼 What I'm Working On Now

> Client work at Zensar Technologies. The code is private, so there are no links here.

### 🔧 Parts Prediction System for Appliance Repair Claims
- **Modelling:** built an ML system that predicts the exact replacement parts a technician needs *before* dispatch, trained on **1.9M+ repair claims**: learning-to-rank (XGBoost, LightGBM LambdaMART) plus a confidence model that scores each part
- **Impact:** beat the incumbent vendor system on **62,967 held-out claims**: **4.5×** top-1 accuracy, **5.7×** more claims with every needed part in the top 5, and **2.6×** precision on high-confidence picks
- **LLM vs ML:** benchmarked Azure OpenAI GPT-6 (alone and with retrieved candidate parts) against the ML model on the same claims; the ML model was **5.6×** more accurate at top-1
- **Deployment:** FastAPI microservice on Kubernetes (Docker, Helm) with an MCP server for an agentic troubleshooting workflow; 100% offline/online parity, 26/26 acceptance tests, plain-English reasons for every prediction
- **MLOps:** config-driven pipeline that works for any appliance: automatic data checks, scheduled retraining (Kubernetes CronJob, GitHub Actions), a promotion gate and versioned releases; training memory cut by **62%**
- **Data quality:** found and fixed **12,872 mislinked label rows** caused by a claim-ID format change, guarded by 22 automated checks

### 🎯 Next Best Offer Recommendation System
- **Entity resolution:** linked **26M claim records** to **40M sales accounts** on Databricks (86.2% verified match vs 15.4% by chance)
- **Customer profiling:** mapped customers to 35 geodemographic personas with confidence scores, feeding the lifetime-value and propensity models

---

## 🚀 Tech Stack & Tools

### 🧠 LLM / GenAI

<p align="left">
  <a href="https://huggingface.co/docs/transformers/model_doc/rag" target="_blank">
    <img src="https://img.shields.io/badge/RAG-000000?style=for-the-badge&logo=searchengineland&logoColor=white" />
  </a>
  <a href="https://huggingface.co/docs/peft/" target="_blank">
    <img src="https://img.shields.io/badge/LoRA%20%2F%20QLoRA-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white" />
  </a>
  <a href="https://huggingface.co/docs/trl/" target="_blank">
    <img src="https://img.shields.io/badge/DPO%20%2F%20SFT-412991?style=for-the-badge&logo=openai&logoColor=white" />
  </a>
  <a href="https://huggingface.co/docs" target="_blank">
    <img src="https://img.shields.io/badge/HuggingFace-FFD21E?style=for-the-badge&logo=huggingface&logoColor=black" />
  </a>
  <a href="https://modelcontextprotocol.io/" target="_blank">
    <img src="https://img.shields.io/badge/MCP-000000?style=for-the-badge&logoColor=white" />
  </a>
  <a href="https://python.langchain.com/" target="_blank">
    <img src="https://img.shields.io/badge/LangChain%20%2F%20LangGraph-1C3C3C?style=for-the-badge&logo=langchain&logoColor=white" />
  </a>
  <a href="https://langfuse.com/docs" target="_blank">
    <img src="https://img.shields.io/badge/Langfuse-000000?style=for-the-badge&logo=grafana&logoColor=white" />
  </a>
  <a href="https://learn.microsoft.com/en-us/azure/ai-services/openai/" target="_blank">
    <img src="https://img.shields.io/badge/Azure%20OpenAI-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white" />
  </a>
  <a href="https://platform.openai.com/docs" target="_blank">
    <img src="https://img.shields.io/badge/OpenAI-412991?style=for-the-badge&logo=openai&logoColor=white" />
  </a>
  <a href="https://docs.anthropic.com/" target="_blank">
    <img src="https://img.shields.io/badge/Anthropic%20Claude-191919?style=for-the-badge&logoColor=white" />
  </a>
  <a href="https://ai.google.dev/" target="_blank">
    <img src="https://img.shields.io/badge/Gemini-4285F4?style=for-the-badge&logo=google&logoColor=white" />
  </a>
  <a href="https://console.groq.com/docs/" target="_blank">
    <img src="https://img.shields.io/badge/Groq-F55036?style=for-the-badge&logoColor=white" />
  </a>
  <a href="https://ollama.com/" target="_blank">
    <img src="https://img.shields.io/badge/Ollama-000000?style=for-the-badge&logoColor=white" />
  </a>
  <a href="https://developers.deepgram.com/" target="_blank">
    <img src="https://img.shields.io/badge/Deepgram-00D4AA?style=for-the-badge&logoColor=white" />
  </a>
  <a href="https://elevenlabs.io/docs" target="_blank">
    <img src="https://img.shields.io/badge/ElevenLabs-000000?style=for-the-badge&logoColor=white" />
  </a>
</p>

---

### 📈 Machine Learning & Ranking

<p align="left">
  <a href="https://xgboost.readthedocs.io/" target="_blank">
    <img src="https://img.shields.io/badge/XGBoost-189FDD?style=for-the-badge&logoColor=white" />
  </a>
  <a href="https://lightgbm.readthedocs.io/" target="_blank">
    <img src="https://img.shields.io/badge/LightGBM-02569B?style=for-the-badge&logoColor=white" />
  </a>
  <a href="https://github.com/catboost/catboost" target="_blank">
    <img src="https://img.shields.io/badge/CatBoost-FFCC00?style=for-the-badge&logoColor=black" />
  </a>
  <a href="https://scikit-learn.org/stable/" target="_blank">
    <img src="https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white" />
  </a>
  <a href="https://shap.readthedocs.io/" target="_blank">
    <img src="https://img.shields.io/badge/SHAP-FF0D57?style=for-the-badge&logoColor=white" />
  </a>
  <a href="https://pandas.pydata.org/docs/" target="_blank">
    <img src="https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white" />
  </a>
  <a href="https://numpy.org/doc/" target="_blank">
    <img src="https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white" />
  </a>
  <a href="https://matplotlib.org/stable/" target="_blank">
    <img src="https://img.shields.io/badge/Matplotlib-11557C?style=for-the-badge&logo=plotly&logoColor=white" />
  </a>
</p>

---

### 🤖 Deep Learning & Vision

<p align="left">
  <a href="https://pytorch.org/docs/stable/" target="_blank">
    <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white" />
  </a>
  <a href="https://www.tensorflow.org/learn" target="_blank">
    <img src="https://img.shields.io/badge/TensorFlow%20%2F%20Keras-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white" />
  </a>
  <a href="https://docs.ultralytics.com/" target="_blank">
    <img src="https://img.shields.io/badge/YOLOv8-000000?style=for-the-badge&logo=opencv&logoColor=white" />
  </a>
  <a href="https://docs.opencv.org/" target="_blank">
    <img src="https://img.shields.io/badge/OpenCV-27338e?style=for-the-badge&logo=opencv&logoColor=white" />
  </a>
</p>

---

### 💻 Programming Languages

<p align="left">
  <a href="https://docs.python.org/3/" target="_blank">
    <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" />
  </a>
  <a href="https://www.w3schools.com/sql/" target="_blank">
    <img src="https://img.shields.io/badge/SQL-003B57?style=for-the-badge&logo=mysql&logoColor=white" />
  </a>
  <a href="https://www.gnu.org/software/bash/manual/" target="_blank">
    <img src="https://img.shields.io/badge/Bash-4EAA25?style=for-the-badge&logo=gnubash&logoColor=white" />
  </a>
  <a href="https://docs.oracle.com/en/java/" target="_blank">
    <img src="https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white" />
  </a>
  <a href="https://cran.r-project.org/" target="_blank">
    <img src="https://img.shields.io/badge/R-276DC3?style=for-the-badge&logo=r&logoColor=white" />
  </a>
  <a href="https://learn.microsoft.com/en-us/dax/" target="_blank">
    <img src="https://img.shields.io/badge/DAX-003B57?style=for-the-badge&logo=microsoft&logoColor=white" />
  </a>
  <a href="https://developer.mozilla.org/en-US/docs/Web/HTML" target="_blank">
    <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" />
  </a>
  <a href="https://developer.mozilla.org/en-US/docs/Web/CSS" target="_blank">
    <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white" />
  </a>
</p>

---

### 🚢 MLOps & Deployment

<p align="left">
  <a href="https://fastapi.tiangolo.com/" target="_blank">
    <img src="https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white" />
  </a>
  <a href="https://docs.docker.com/" target="_blank">
    <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" />
  </a>
  <a href="https://kubernetes.io/docs/" target="_blank">
    <img src="https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white" />
  </a>
  <a href="https://helm.sh/docs/" target="_blank">
    <img src="https://img.shields.io/badge/Helm-0F1689?style=for-the-badge&logo=helm&logoColor=white" />
  </a>
  <a href="https://docs.github.com/en/actions" target="_blank">
    <img src="https://img.shields.io/badge/GitHub%20Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white" />
  </a>
  <a href="https://git-scm.com/doc" target="_blank">
    <img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white" />
  </a>
  <a href="https://docs.railway.app/" target="_blank">
    <img src="https://img.shields.io/badge/Railway-0B0D0E?style=for-the-badge&logo=railway&logoColor=white" />
  </a>
  <a href="https://vercel.com/docs" target="_blank">
    <img src="https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white" />
  </a>
</p>

---

### 📊 Data & Analytics

<p align="left">
  <a href="https://docs.databricks.com/" target="_blank">
    <img src="https://img.shields.io/badge/Databricks-FF3621?style=for-the-badge&logo=databricks&logoColor=white" />
  </a>
  <a href="https://neo4j.com/docs/" target="_blank">
    <img src="https://img.shields.io/badge/Neo4j-4581C3?style=for-the-badge&logo=neo4j&logoColor=white" />
  </a>
  <a href="https://learn.microsoft.com/en-us/power-bi/" target="_blank">
    <img src="https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black" />
  </a>
  <a href="https://help.tableau.com/" target="_blank">
    <img src="https://img.shields.io/badge/Tableau-E97627?style=for-the-badge&logo=tableau&logoColor=white" />
  </a>
  <a href="https://docs.jupyter.org/" target="_blank">
    <img src="https://img.shields.io/badge/Jupyter-FA0F00?style=for-the-badge&logo=jupyter&logoColor=white" />
  </a>
  <a href="https://colab.research.google.com/" target="_blank">
    <img src="https://img.shields.io/badge/Google%20Colab-F9AB00?style=for-the-badge&logo=googlecolab&logoColor=black" />
  </a>
</p>

---

### ☁️ Cloud & Compute

<p align="left">
  <a href="https://learn.microsoft.com/en-us/azure/" target="_blank">
    <img src="https://img.shields.io/badge/Azure-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white" />
  </a>
  <a href="https://docs.aws.amazon.com/" target="_blank">
    <img src="https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazonaws&logoColor=white" />
  </a>
  <a href="https://cloud.google.com/docs" target="_blank">
    <img src="https://img.shields.io/badge/GCP-4285F4?style=for-the-badge&logo=googlecloud&logoColor=white" />
  </a>
  <a href="https://docs.oracle.com/en/cloud/" target="_blank">
    <img src="https://img.shields.io/badge/Oracle%20Cloud-FF0000?style=for-the-badge&logo=oracle&logoColor=white" />
  </a>
  <a href="https://www.amd.com/en/products/accelerators/instinct/mi300/mi300x.html" target="_blank">
    <img src="https://img.shields.io/badge/AMD%20MI300X-ED1C24?style=for-the-badge&logo=amd&logoColor=white" />
  </a>
</p>

---

## 💡 About Me

💼 AI Engineer at Zensar Technologies, building production ML and LLM systems for a Fortune 500 insurance client. I've taken a model from raw warehouse data to a live Kubernetes service with automated retraining.

**What I focus on:**
- 🎯 **Ranking & Recommendation** — learning-to-rank, calibrated probabilities, honest held-out evaluation
- 🚢 **MLOps** — FastAPI services, Docker, Kubernetes, Helm, scheduled retraining, versioned releases
- 🔍 **RAG & Retrieval** — hybrid BM25 + vector search, LLM reranking, multi-provider routing, CI eval gates
- 🧬 **LLM Fine-Tuning** — LoRA, QLoRA, DPO on AMD MI300X (192 GB VRAM); real negative results documented
- ⚖️ **LLM vs ML Benchmarking** — measuring where LLMs actually add value, with evidence
- 📊 **Observability** — Langfuse tracing, p50/p95 latency per step, automatic quality regression checks

**Also strong in:**
- 📊 Data Analysis & Visualisation — EDA, data validation, dashboards, Power BI, Tableau
- 🤖 Deep Learning — CNNs, YOLOv8, transfer learning
- 🔗 Data Engineering — ETL pipelines, entity resolution, datasets with millions of records

---

## 💻 Featured Projects

### 🤖 Production RAG System — Ask My Docs 🔗 [GitHub](https://github.com/Kkj1203/RAG_AskMyDocs)

- Hybrid retrieval (70% vector + 30% BM25, top-10) with LLM reranking (top-10 → top-5); session-isolated multi-PDF ingestion with 6-turn chat memory
- 5-provider LLM fallback router (Groq → OpenRouter → Gemini → OpenAI → Anthropic); Langfuse tracing: rerank p50 = 5.95 s, total p50 = 11.09 s
- GitHub Actions CI gate — runs a token-overlap eval on every push; blocks merge if the quality score is below 0.4

---

### 🧬 LLM Fine-Tuning: SFT + DPO Pipeline 🔗 [GitHub](https://github.com/Kkj1203/LLMFineTuningLoRA)

- Fine-tuned Phi-3-mini-4k-instruct (3.8B) for JSON extraction — LoRA r=16, 0.23% trainable params; overall score 0.544 → 0.870 (+60%), format compliance 50% → 100% on AMD MI300X (bf16)
- Custom DPO training loop in pure PyTorch (500 pairs, 63 s, $1.99/hr); documented negative result — domain-mismatched preference data causes task regression
- Prototyped on Colab T4 (32 s, free), scaled to AMD MI300X via Docker/ROCm

---

### 🎙️ Real-Time Voice RAG Assistant 🔗 [GitHub](https://github.com/Kkj1203/VoiceRAGAssistant)

- Voice-to-voice pipeline: Deepgram STT (3.1 s) → RAG retrieval (19.9 s) → ElevenLabs TTS (5.6 s) → MP3; total latency 28.7 s with per-stage graceful degradation
- Stateless voice middleware over the RAG API; custom ElevenLabs Voice Lab voice
- Benchmarked 3 local small language models via Ollama across 5 task categories ([Local SLM Benchmark](https://github.com/Kkj1203/Local_SLM_Benchmark))

---

### 😄 Facial Emotion Recognition using CNN (DenseNet Transfer Learning) 🔗 [GitHub](https://github.com/Kkj1203/Facial-Emotion-Recognition-CNN-DenseNet)

- Built a deep learning model to classify 7 facial emotions using the FER-2013 dataset
- Applied transfer learning with DenseNet169 and fine-tuning for better generalisation
- Evaluated with accuracy, confusion matrix and ROC–AUC

---

### 🌱 YOLOv8-based Crop Disease Detection System 🔗 [GitHub](https://github.com/Kkj1203/YOLOv8-CropDiseasePredictor)

- End-to-end object detection pipeline for multi-class crop disease identification
- Fine-tuned YOLOv8 Nano from pretrained weights on a custom dataset (10 classes, 2,000+ images); mAP@0.5 = 0.80, real-time at 30+ FPS
- Assessed with precision, recall and mAP

---

### 🚑 SETU — Smart Emergency Triage System (IEEE ICTBIG) 🔗 [GitHub](https://github.com/Kkj1203/SETU-final)

- IoT emergency response system linking biometric identification with cloud health records; hospital allocation within 120 seconds
- Co-authored an IEEE paper published at ICTBIG; Top 20 of 600+ teams at Smart India Hackathon

---

### 📊 Vendor Performance Analytics 🔗 [GitHub](https://github.com/Kkj1203/Vendor-Performance-Analytics)

- Integrated 6 vendor datasets (1M+ records) using Python and SQL with schema standardisation via ETL
- Built a Power BI dashboard tracking 5+ KPIs for vendor evaluation and decision support

---

### 🌐 Social Sphere – Text-based Social Media Platform 🔗 [GitHub](https://github.com/Kkj1203/SocialSphere)

- Full-stack Java EE web application with secure authentication, post creation, feeds and comments
- Used JSP, Servlets, JDBC and MVC principles for a scalable design

---

<h3 align="center">
  <b>🚀 More projects →</b>
  <a href="https://github.com/Kkj1203?tab=repositories">View all repositories</a>
</h3>

---

## 📈 GitHub Stats

<p align="center">
  <img src="https://github.com/Kkj1203/Kkj1203/blob/main/github-metrics.svg" />
</p>

---

## 🐍 Contribution Snake

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)"
      srcset="https://github.com/Kkj1203/Kkj1203/blob/output/github-contribution-grid-snake-dark.svg" />
    <source media="(prefers-color-scheme: light)"
      srcset="https://github.com/Kkj1203/Kkj1203/blob/output/github-contribution-grid-snake.svg" />
    <img alt="github contribution grid snake animation"
      src="https://github.com/Kkj1203/Kkj1203/blob/output/github-contribution-grid-snake.svg" />
  </picture>
</p>

---

## 📫 Connect with Me

<p align="center">
  <a href="https://www.linkedin.com/in/keerthikrishna-jog-93b6321b9" target="_blank">
    <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" />
  </a>
  <a href="https://github.com/Kkj1203" target="_blank">
    <img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" />
  </a>
  <a href="mailto:keerthikrishnajog120304@gmail.com">
    <img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" />
  </a>
</p>

---

🔍 *Open to full-time roles in AI Engineering, Machine Learning and LLM systems.*
