# Hey, I'm Mariah

I'm a Computer Science and Data Science graduate of the University of Wisconsin–River Falls (September 2026), interested in machine learning, data science, and backend software engineering.

I've deployed machine learning models into a production database at a 500K-member credit union, run applied ML experiments from data preparation through evaluation, and built and shipped software from APIs to a live consumer app. I care about honest evaluation: baselines, held-out data, and reporting results even when they're not flattering.

Open to Data Scientist, Data Analyst, Backend Software Engineer, and ML/AI Engineer roles in Minnesota, Wisconsin, Illinois, or remote, and willing to relocate.

## Selected projects

### [Remmebr](https://remmebr.com): AI study and career-prep platform

Remmebr is a live study and learning platform built around spaced repetition, active recall, practice testing, and source-grounded AI tools. It runs on web, iOS/iPadOS, Android, and as a desktop PWA, with subscriptions through Stripe and StoreKit 2.

I'm the founder and product lead. I define the roadmap and system design and direct AI-assisted development (GitHub Copilot, Cursor, OpenCode), with written engineering standards and an AI-agent guide that I review the generated code against. I also handle go-to-market myself: App Store positioning, landing page, press kit, and short-form video.

Career-prep features (job-posting analysis, resume tailoring, job-specific interview prep) are currently in development.

**Stack:** JavaScript, Supabase/PostgreSQL, Vercel, Stripe, StoreKit 2, AI and document-processing APIs

The production repository is private.

### [Loan Default Prediction System](https://github.com/mariahwaslie/Loan-Default-Prediction-System-)

An end-to-end default-risk system on about 1.27 million LendingClub loans.

- Removed post-origination leakage fields and used chronological train, validation, and test splits (2012–16, 2017, 2018) instead of random splitting.
- Compared logistic regression, random forest, XGBoost, LightGBM, and CatBoost; tuned CatBoost with Optuna, reduced 93 candidate predictors to 75 with SHAP, calibrated probabilities with isotonic regression, and chose the threshold on validation data.
- Held-out 2018 results: ROC-AUC 0.7531 (95% bootstrap CI 0.748–0.759), PR-AUC 0.3506, F1 0.402, Brier score 0.1151.
- Served through a FastAPI endpoint with a React/Vite interface and Docker Compose, with a Pytest suite (model artifacts, inference behavior, preprocessing, API routes) run in GitHub Actions CI.

**Stack:** Python, CatBoost, LightGBM, XGBoost, Scikit-learn, SHAP, Optuna, FastAPI, React, Docker, Pytest

### [ML-Guided SSD Garbage Collection](https://github.com/mariahwaslie/ML-SSD-Garbage-Collection)

An operating-systems experiment (UWRF CIDS 429) that extends the OSTEP SSD simulator with an optional ML policy for choosing which flash block to clean, kept behind a feature switch so the original collector stays available for A/B comparison.

Across 54 seeded runs plus skewed workloads, the ML policy cut estimated time 2.4% in the smallest configuration but ran up to about 28% slower in larger ones because it triggered more erases. The write-up explains why erase cost dominates.

**Stack:** Python, Scikit-learn

### [VM Page Replacement with LSTM Prediction](https://github.com/mariahwaslie/VM-Page-Replacement-Policy-RNN)

An operating-systems project (UWRF CIDS 429) that adds a PyTorch LSTM eviction policy to the OSTEP paging simulator. The model predicts which pages will be reused in the next 10 accesses and evicts the page with the lowest predicted reuse.

I trained 42 model variants and compared the best against FIFO, LRU, CLOCK, RAND, and OPT on identical address streams. Average hit rate was 89.3% vs. 88.6% for LRU on an 80/20 locality workload, and 63.5% vs. 50.7% for FIFO/LRU on a looping workload.

**Stack:** Python, PyTorch

### [AI Reading Companion](https://github.com/mariahwaslie/ai-reading-companion)

[Try it live](https://ai-reading-companion.streamlit.app)

A RAG application for asking questions about uploaded PDF and EPUB documents. It uses Hugging Face Sentence Transformers for semantic scoring to retrieve relevant passages, then grounds answers in those passages with citations.

**Stack:** Python, LangChain, ChromaDB, Hugging Face Sentence Transformers, OpenAI, Streamlit

### [Social Media Platform](https://github.com/mariahwaslie/socialmedia-app)

A full-stack Django application (8 apps) covering posts, media, blogs, groups, events, direct messaging, boards, playlists, cross-model search, and a TF-IDF recommender. Real-time chat and notifications run on Django Channels, WebSockets, and Redis, and the project includes role-based permissions and privacy controls.

**Stack:** Python, Django, Django Channels, Redis, Docker, Scikit-learn

### Clinical Deterioration Early Warning Platform (in progress)

A FHIR-compliant clinical risk API with 12+ REST endpoints across 6 resource types (Patient, Encounter, Observation, Condition, MedicationRequest, RiskAssessment), built on Spring Boot and PostgreSQL with JWT authentication (Spring Security), a layered DTO/mapper design, and JUnit tests. It's loaded with synthetic Synthea data. Time-series deterioration models and Kubernetes deployment are planned, not yet built. The repository is private.

**Stack:** Java, Spring Boot, PostgreSQL, Spring Security, JUnit, FHIR

### [Weekly AI News Digest](https://github.com/mariahwaslie/focuskpi-news-digest)

An n8n workflow (built for a FocusKPI take-home) that pulls three RSS feeds each Monday, cleans and dedupes them in code, and has an LLM pick 3–5 takeaways to post to Slack.

**Stack:** n8n, OpenAI API, JavaScript

### Serverless Video-to-Quiz Pipeline

An event-driven AWS pipeline built with Java CDK: uploading a video to S3 triggers Transcribe, a Bedrock model generates a structured quiz, and the result is written back to S3. Infrastructure is defined as code with Lambda, S3, IAM, and AWS CDK.

### [Deep Q-Network OS Scheduler](https://github.com/mariahwaslie/mlfq)

A PyTorch reinforcement learning project for CPU scheduling in a multi-level feedback queue simulation, with a state and reward design around throughput, responsiveness, and starvation, compared with FIFO and Round-Robin.

## Technical background

**Machine learning:** Python, PyTorch, TensorFlow/Keras, Scikit-learn, XGBoost, LightGBM, CatBoost, SHAP, Optuna, Hugging Face (Sentence Transformers, semantic scoring), LangChain, RAG, NumPy, Pandas

**Backend:** Java (Spring Boot), Django, FastAPI, Flask, Redis, WebSockets, REST APIs, SQLAlchemy, Pydantic

**Cloud and infrastructure:** AWS (Lambda, S3, CDK, Transcribe, Bedrock), Vercel, Docker, GitHub Actions, Azure DevOps, Git

**Systems and testing:** Linux, bash, C (operating-systems programming), Pytest, JUnit

**Data:** PostgreSQL, Oracle SQL, SQLite, Supabase, ChromaDB

**AI-assisted development:** GitHub Copilot, Cursor, OpenCode, OpenAI and DeepSeek APIs

**Languages:** Python, Java, SQL, R, C, JavaScript, HTML/CSS

## Experience

**Advanced Analytics Intern, Royal Credit Union** (May–Sep 2025): built and deployed churn-prediction and product-recommendation models into a production Oracle database. Featured in a [UW–Eau Claire story](https://www.uwec.edu/stories/royal-credit-union-teams-three-campuses-ai-solutions) on the team's AI work.

## Contact

[LinkedIn](https://www.linkedin.com/in/mariahwaslie) · [Portfolio](https://mariahwaslie.github.io/) 

B.S. Computer Science and Data Science, University of Wisconsin–River Falls, September 2026
