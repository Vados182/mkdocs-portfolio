# Hi, I'm Wadim! 👋

I am a **Data Scientist** with a strong background in building production ML applications and GenAI/RAG solutions. Experienced across the full data product lifecycle—from advanced analytics (SQL, DuckDB, PySpark) to deploying containerized services (FastAPI, Docker, Render) with complete CI/CD pipelines, computer vision (PyTorch), and model observability.

---

## 🚀 About Me
I focus on turning raw data into valuable decisions and fully automated data products. My approach combines advanced machine learning, predictive modeling, and generative AI with scalable cloud infrastructure.

> **My Approach:** *"Data speaks for itself if you know how to ask it questions."*

---

## 🛠️ Featured Projects

| Project | Description | Main Technologies |
| :--- | :--- | :--- |
| **[Multimodal E-Commerce Intelligence Platform](#multimodal-e-commerce-intelligence-platform)** | Production analytical platform integrating PySpark ETL, GenAI agents, PyTorch computer vision, and causal inference. | Python, FastAPI, PySpark, PyTorch, OpenAI API, Streamlit, Docker, GitHub Actions |
| **[MLOps & GenAI Customer Retention Platform](#mlops--genai-customer-retention-platform)** | End-to-end churn prediction pipeline with dynamic LLM retention messaging. | Python, XGBoost, Azure ML, FastAPI, Docker, Render, GitHub Actions |
| **[TikTok AI Analytics & Automated Pipeline](#tiktok-ai-analytics--automated-pipeline)** | Automated ingestion, GenAI sentiment analysis, and live Streamlit dashboard. | Python, Gemini API, PostgreSQL, Streamlit, GitHub Actions, Render |
| **[Warsaw Real Estate Price Predictor](#warsaw-real-estate-price-predictor-production-rest-api--mlllm)** | Production REST API with LLM parameter extraction, inference, and Langfuse tracking. | Python, FastAPI, PyCaret, GPT-4o-mini, Langfuse, Docker, Render |
| **[Warsaw Real Estate Price Calculator](#warsaw-real-estate-price-calculator)** | Interactive web app estimating Warsaw property values from raw descriptions. | Python, PyCaret, Streamlit, Langfuse, GenAI |
| **[EDA & RFM Customer Segmentation](#eda-and-rfm-customer-segmentation-olist)** | DuckDB SQL analysis of 100k+ e-commerce orders for customer categorization. | Python, DuckDB, SQL, Pandas, Seaborn |
| **[New York Airbnb Market Analysis](#new-york-airbnb-market-analysis)** | Hybrid Python & DuckDB SQL analysis of 48k+ short-term rental records. | Python, DuckDB, SQL, Pandas, Matplotlib |
| **[Multimedia Chatbot Assistant (RAG)](#multimedia-chatbot-assistant-rag)** | Streamlit application with model switching and multi-format document RAG analysis. | Python, Streamlit, OpenAI API, RAG, pypdf |
| **[AI Video Subtitle Generator](#ai-video-subtitle-generator)** | Web tool automating subtitle generation, translation, editing, and video burning. | Python, Streamlit, OpenAI Whisper, GPT-4, FFmpeg |

---

## 📌 Projects Detail

### Multimodal E-Commerce Intelligence Platform
A production-ready analytical system designed for e-commerce intelligence that combines distributed data pipelines, computer vision, generative AI, and causal analytics into a unified microservice architecture.
- **Skills**: Python, FastAPI, PySpark, PyTorch (`MobileNetV3`), Causal Inference, OpenAI API, Streamlit, Docker, GitHub Actions (CI/CD)
- **Result**: Engineered a resource-optimized FastAPI microservice (512MB RAM constraint on Render) backed by a PySpark ETL pipeline exporting to Parquet storage, integrated with a PyTorch image classifier and GenAI product categorization agent featuring automatic fallback mocks.

### MLOps & GenAI Customer Retention Platform
End-to-end production pipeline for predicting e-commerce customer churn and automatically generating GenAI retention strategies.
- **Skills**: Python, XGBoost, Optuna, SHAP, Azure ML Workspace, OpenAI API, FastAPI, Docker, Render, GitHub Actions (CI/CD)
- **Result**: Deployed a containerized FastAPI service on Render integrated with GitHub Actions CI/CD; automated churn prediction and dynamic LLM retention messaging with Azure ML experiment tracking.

### TikTok AI Analytics & Automated Pipeline
An end-to-end automated system that ingests TikTok content, performs GenAI sentiment analysis and summarization, and updates a live cloud database.
- **Skills**: Python, Google Gemini API, PostgreSQL, Psycopg2, Streamlit, Plotly, GitHub Actions, Render
- **Result**: Built an automated CI/CD pipeline via GitHub Actions that analyzes unread social posts daily using Gemini LLM and renders real-time insights on a live Streamlit dashboard.

### Warsaw Real Estate Price Predictor (Production REST API & ML/LLM)
An end-to-end cloud-hosted REST API for estimating property values in the Warsaw real estate market, combining traditional machine learning with GenAI feature extraction and LLM observability.
- **Skills**: Python, FastAPI, PyCaret, OpenAI (GPT-4o-mini), Instructor, Pydantic, Langfuse, Docker, Render, Swagger UI
- **Result**: Built a fully observable production API that extracts structured parameters from raw Polish listing text and predicts property prices with low-latency inference and monitored token consumption.

### Warsaw Real Estate Price Calculator
An end-to-end web application for estimating property values in the Warsaw market, combining traditional machine learning with GenAI technologies to parse raw listing descriptions.
- **Skills**: Python, PyCaret, Streamlit, Langfuse, GenAI
- **Result**: Automated initial property valuation and significantly saved time through intelligent processing of unstructured text.

### EDA and RFM Customer Segmentation (Olist)
Comprehensive exploratory data analysis of over 100k orders from a Brazilian e-commerce platform using the DuckDB SQL engine and an RFM segmentation model.
- **Skills**: Python, DuckDB, SQL, Pandas, Seaborn
- **Result**: Identified logistical bottlenecks and categorized the customer base into strategic groups (e.g., Champions, At Risk) to optimize marketing efforts.

### New York Airbnb Market Analysis
Exploratory data analysis (EDA) of short-term rental data (48k+ records) conducted in a hybrid Python and DuckDB SQL environment.
- **Skills**: Python, DuckDB, SQL, Pandas, Matplotlib
- **Result**: Developed key insights regarding pricing structure, factors driving listing popularity, and effective market anomaly detection.

### Multimedia Chatbot Assistant (RAG)
A Streamlit web application integrated with the OpenAI API, offering real-time dynamic LLM model switching and multi-format document analysis (PDF, DOCX, TXT).
- **Skills**: Python, Streamlit, OpenAI API, RAG, pypdf
- **Result**: Increased user productivity through instant synthesis of knowledge from corporate documentation while maintaining session context.

### AI Video Subtitle Generator
A web tool automating the process of generating, translating, interactively editing, and hardcoding subtitles into video materials.
- **Skills**: Python, Streamlit, OpenAI Whisper, GPT-4, FFmpeg
- **Result**: Drastic reduction in video post-production time and costs, facilitating global content localization.

---

## 🛠️ Technical Skills

* **Programming Languages:** Python, SQL
* **Data & Big Data:** PySpark, Pandas, DuckDB, SQLite, QDrant, Pydantic, PostgreSQL, Psycopg2, Parquet
* **Machine Learning, Deep Learning & AI:** PyTorch (`torchvision`), Causal Inference, Google Gemini API, OpenAI API, XGBoost, Optuna, SHAP, Azure Machine Learning, PyCaret, Instructor, LangChain, Langfuse
* **Visualization & Apps:** FastAPI (REST API), Streamlit, Plotly, Matplotlib, Seaborn, Jupyter
* **Tools & Methodology:** Git, GitHub Actions (CI/CD), VS Code, Agile, Scrum, Kanban, Trello, Jira, Anaconda, ERP Systems
* **Cloud & DevOps:** Docker, Render, AWS, DigitalOcean

---

### My Core Areas of Expertise

<div class="grid cards" markdown>

-   **Advanced Analytics & Data Engineering**
    ---
    ETL pipelines with PySpark, Parquet storage, RFM segmentation, and high-performance querying using DuckDB and PostgreSQL.
    
-   **Machine Learning, Deep Learning & MLOps**
    ---
    Building predictive models, computer vision classifiers (PyTorch), hyperparameter tuning (Optuna), experiment tracking (Azure ML), and model explainability (SHAP).

-   **GenAI, RAG & LLM Observability**
    ---
    Developing RAG applications, LLM agents with fallback architectures, structured output extraction (Instructor/Pydantic), and monitoring token consumption with Langfuse.

-   **Cloud Deployment & CI/CD**
    ---
    Containerizing applications with Docker and building automated CI/CD deployment pipelines using GitHub Actions, FastAPI REST APIs, Streamlit, and Render.

</div>

---

## 📬 Contact
I am always open to discussing Data Science projects, machine learning architectures, collaboration opportunities, or sharing experience!

*   **GitHub:** [github.com/Vados182](https://github.com/Vados182)
*   **LinkedIn:** [linkedin.com/in/wadim-worobiow-226a58147](https://linkedin.com/in/wadim-worobiow-226a58147)
*   **E-mail:** bassuha@gmail.com