# 👋 Hey, I'm Mariah

I like building things that sit at the intersection of data, intelligence, and real impact. I'm a Computer Science & Data Science graduate from the University of Wisconsin–River Falls (August 2026) with a genuine passion for machine learning and software engineering — the kind of work where you take a hard problem, build something that actually solves it, and deploy it somewhere real people use it.

---

## 🚀 Featured Projects

### 📖 AI Reading Companion — Live Deployed
A deployed RAG (Retrieval-Augmented Generation) web app that lets users upload any PDF or EPUB document and ask questions about it. Built with LangChain, ChromaDB, Sentence Transformers, and OpenAI. Every answer is grounded in retrieved document chunks with citations to reduce hallucinations.

🔗 **[Try it live →](https://ai-reading-companion.streamlit.app)**

- 🧠 RAG pipeline with semantic search over document chunks
- 🔍 Local embeddings via `BAAI/bge-base-en-v1.5` (Sentence Transformers)
- 🗄️ ChromaDB vector store for similarity search
- 📄 PDF + EPUB parsing with pypdf, EbookLib, BeautifulSoup
- ✂️ LangChain RecursiveCharacterTextSplitter for context-aware chunking
- 🎯 Prompt engineering for grounded answers with chunk citations
- 🚀 Deployed on Streamlit Community Cloud

---

### 🌐 Social Media Platform
A full-stack Django 4.2 platform with real-time WebSocket messaging, TF-IDF recommendation engine, role-based authentication, and API integration — entirely self-directed over one summer.

- ⚡ Real-time messaging via Django Channels, WebSockets, and Redis
- 🔐 JWT authentication, role-based groups, privacy controls
- 🤖 TF-IDF cosine similarity recommendation engine with Scikit-learn
- 📖 API with database seeding management commands

---

### ☁️ Serverless Video-to-Quiz Pipeline
An event-driven serverless data pipeline on AWS built with Java CDK. A video uploaded to S3 triggers Lambda → AWS Transcribe for speech-to-text → AWS Bedrock LLM generates a structured quiz written back to S3. Zero manual AWS Console setup.

- 🏗️ All infrastructure provisioned as code with AWS CDK
- 🎙️ AWS Transcribe for speech-to-text conversion
- 🤖 AWS Bedrock LLM for structured quiz generation
- ☁️ Lambda, S3, IAM — fully serverless architecture

---

### 🧠 Deep Q-Network OS Scheduler
A DQN reinforcement learning agent built in PyTorch from scratch to learn optimal CPU scheduling policies for a multi-level feedback queue simulation — benchmarked against FIFO and Round-Robin baselines.

- 🎯 Custom reward function balancing throughput, responsiveness, and starvation
- 📈 State vector engineered from 10+ system signals
- ⚖️ Benchmarked against industry-standard scheduling algorithms

---

### 🎵 AI Audio Analysis — Whisper Transcription & Study Guide Generator
A Streamlit app that downloads YouTube audio via yt-dlp, transcribes it using OpenAI Whisper, and generates structured study notes and summaries via the OpenAI Chat API.

- 📥 YouTube audio download and processing via yt-dlp and FFmpeg
- 🎙️ OpenAI Whisper API for audio transcription
- 📝 OpenAI Chat API for structured study note generation
- 🔧 Handles M3U8 streams and Selenium-based lecture video extraction

---

### 🌌 NASA Space Image & News App — Live Deployed
A deployed Streamlit application fetching NASA's Astronomy Picture of the Day via the NASA APOD API with date selection, and scraping NASA news articles using BeautifulSoup.

- 🔭 NASA APOD API integration with date-parameterized calls
- 📰 NASA news scraping with BeautifulSoup and Requests

---

## 🛠️ My Tech Stack

**ML & AI**: Python · PyTorch · TensorFlow/Keras · Scikit-learn · XGBoost · LightGBM · HuggingFace · Sentence Transformers · LangChain · ChromaDB · RAG · MLflow · OpenAI API · NumPy · Pandas

**Backend**: Django · Django Channels · FastAPI · Flask · Redis · WebSockets · RESTful APIs · SQLAlchemy · Pydantic

**Cloud & DevOps**: AWS (Lambda · S3 · EC2 · Transcribe · Bedrock · CDK) · Azure · Docker · Git · Infrastructure as Code · Azure DevOps

**Databases**: PostgreSQL · Oracle SQL · SQLite · ChromaDB · Django ORM · SQLAlchemy ORM

**Languages**: Python · Java · SQL · R · C · JavaScript · HTML/CSS

---

## 📫 Let's Connect

- 💼 LinkedIn: [linkedin.com/in/mariah-w-3b97b9233](https://www.linkedin.com/in/mariah-w-3b97b9233)
- 📍 Open to relocation — Raleigh-Durham · Boston · Chicago · Minneapolis · Madison · Remote
- 🎓 Available August 2026

---

*Open to MLE, backend SWE, and data engineering roles. If something in my work looks interesting to you, feel free to reach out.*
