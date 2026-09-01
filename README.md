# Hey, I'm Mariah

I'm a Computer Science and Data Science graduate from the University of Wisconsin-River Falls. My work is mostly in machine learning and software engineering.

I've spent much of the past year building [Remmebr](https://remmebr.com), a study platform that grew from a personal project into a production application. I also work on applied machine learning projects where the focus is not just training a model, but getting the evaluation and deployment decisions right.

## 🚀 Selected projects

### Remmebr

[remmebr.com](https://remmebr.com)

Remmebr is a study and learning platform built around spaced repetition, active recall, practice testing, course materials, and AI-assisted learning.

I built the application across web, iOS/iPadOS, Android, and desktop PWA. It includes adaptive study planning, document processing, source-grounded AI tools, coursework and assignment features, handwriting support, authentication, subscriptions, cloud storage, and persistent user data.

The stack includes JavaScript, Supabase/PostgreSQL, Vercel, Stripe, StoreKit 2, and AI and document-processing APIs.

The production repository is private. The application is live at [remmebr.com](https://remmebr.com).

### Loan Default Risk Modeling

An applied machine learning pipeline for predicting LendingClub loan defaults using historical borrower, loan, and credit data.

The modeling dataset contains about 1.27 million loans. I used chronological train, validation, and test splits rather than random splitting so evaluation better matches how a credit-risk model would be used on future loans.

I removed post-origination leakage fields before training, compared several model families, used SHAP to reduce the feature set, calibrated the final CatBoost model with isotonic regression, and selected the classification threshold on the validation set.

Final holdout performance:

- ROC-AUC: 0.7531
- PR-AUC: 0.3506
- F1: 0.4020
- Brier score: 0.1151
- 95% bootstrap ROC-AUC interval: 0.748 to 0.759

The final artifact packages the calibrated model, selected features, categorical feature list, and decision threshold for inference.

**Stack:** Python, CatBoost, LightGBM, XGBoost, Scikit-learn, SHAP, Optuna, Pandas, NumPy

### AI Reading Companion

[Try it live](https://ai-reading-companion.streamlit.app)

A RAG application for asking questions about uploaded PDF and EPUB documents. It retrieves relevant passages with semantic search and grounds answers in those passages with citations.

Built with Python, LangChain, ChromaDB, Sentence Transformers, OpenAI, pypdf, EbookLib, BeautifulSoup, and Streamlit.

### Serverless Video-to-Quiz Pipeline

An event-driven AWS pipeline built with Java CDK.

Uploading a video to S3 triggers transcription through AWS Transcribe, sends the transcript to an AWS Bedrock model, generates a structured quiz, and writes the result back to S3.

The infrastructure is provisioned in code with Lambda, S3, IAM, Transcribe, Bedrock, and AWS CDK.

### Deep Q-Network OS Scheduler

A PyTorch reinforcement learning project for CPU scheduling in a multi-level feedback queue simulation.

I designed the state representation and reward function around throughput, responsiveness, and starvation, then compared the learned policy with FIFO and Round-Robin schedulers.

### Social Media Platform

A Django 4.2 application with real-time messaging through Django Channels, WebSockets, and Redis.

It also includes JWT authentication, role-based permissions, privacy controls, an API, and a TF-IDF recommendation system built with Scikit-learn.

## 🛠 Technical background

**Machine learning:** Python, PyTorch, TensorFlow/Keras, Scikit-learn, XGBoost, LightGBM, CatBoost, Hugging Face, Sentence Transformers, SHAP, Optuna, LangChain, RAG, MLflow, NumPy, Pandas

**Backend:** Django, FastAPI, Flask, Redis, WebSockets, REST APIs, SQLAlchemy, Pydantic

**Cloud and infrastructure:** AWS, Azure, Vercel, Docker, Git, AWS CDK, Infrastructure as Code, Azure DevOps

**Data:** PostgreSQL, Oracle SQL, SQLite, ChromaDB, Supabase

**Languages:** Python, Java, SQL, R, C, JavaScript, HTML/CSS

## 📫 Contact

[LinkedIn](https://www.linkedin.com/in/mariahwaslie)

B.S. Computer Science and Data Science, University of Wisconsin-River Falls, August 2026

Open to relocation and interested in machine learning engineering, backend software engineering, and related roles.
