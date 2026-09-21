# 🛒 MLOps & GenAI Customer Retention Platform

2026-09-21

![CI/CD Pipeline](https://github.com/Vados182/MLOps-GenAI-E-Commerce-Platform/actions/workflows/cicd.yml/badge.svg)

An enterprise-grade, end-to-end Machine Learning and Generative AI system designed to predict customer churn risk for e-commerce platforms (based on the Olist Brazilian dataset) and automatically orchestrate targeted, personalized retention campaigns using large language models.

---

## 🔗 Live Links & Architecture

* **Live Interactive API (Swagger UI)**: [https://olist-churn-api.onrender.com/docs](https://olist-churn-api.onrender.com/docs)
* **GitHub Repository**: [https://github.com/Vados182/MLOps-GenAI-E-Commerce-Platform](https://github.com/Vados182/MLOps-GenAI-E-Commerce-Platform)
* **Docker Container Registry**: Hosted on Render Cloud

---

## 💡 Executive Summary

Customer churn is one of the most critical metrics in e-commerce. Retaining an existing customer is significantly cheaper than acquiring a new one. 

This platform bridges classical predictive Machine Learning with modern Generative AI:
1. **Predictive Modeling**: Analyzes transactional, logistical, and behavioral features to produce a high-precision churn probability score.
2. **Generative Automation**: If the predicted churn risk exceeds the threshold (`is_high_risk: true`), an automated LLM agent dynamically crafts a personalized, empathetic compensation message and discount strategy tailored to the customer's specific grievance (e.g., severe delivery delays or high freight costs).

---

## 🛠️ Complete Tech Stack & Tools

### 1. **Data Engineering & Exploratory Analysis**
* **Python 3.11**: Core programming language.
* **Pandas & NumPy**: Feature engineering, data cleansing, and tabular transformations.
* **DuckDB & SQL**: High-performance analytical queries executed on 100k+ historical order records.
* **SHAP (SHapley Additive exPlanations)**: Model explainability and feature importance analysis to identify key drivers of churn (e.g., `delivery_diff_days`, `total_freight_value`).

### 2. **Machine Learning & Experimentation**
* **XGBoost**: Gradient boosted decision tree framework trained to classify customer churn.
* **Optuna**: Automated Hyperparameter Optimization (HPO) for tuning tree depth, learning rates, and regularization parameters.
* **Azure Machine Learning Workspace**: Cloud-based experiment tracking, run logging, metrics logging, and artifact management.

### 3. **Generative AI & LLM Orchestration**
* **OpenAI API (`gpt-4o-mini` / `gpt-4o`)**: Generates real-time, context-aware retention offers.
* **Pydantic v2**: Strict schema validation and structured JSON output enforcing type safety for LLM payloads.

### 4. **Backend API Development**
* **FastAPI**: Asynchronous Python web framework delivering low-latency inference endpoints (`/predict` and `/predict-with-retention`).
* **Uvicorn**: Lightning-fast ASGI web server implementation.
* **Swagger UI / OpenAPI 3.1**: Auto-generated interactive API documentation.

### 5. **DevOps, Containerization & CI/CD**
* **Docker**: Single-file multi-stage containerization ensuring environment reproducibility across local and cloud environments.
* **Render**: Cloud platform hosting the live Dockerized application with environment variable configuration for API key security.
* **GitHub Actions**: Automated CI/CD workflow executing Python syntax checking (`flake8` linting) and triggering production deployment via Render Deploy Hooks upon every push to `main`.
* **Git**: Version control following semantic commit conventions.

---

## 📐 System Architecture & Flow

```
[ Customer Data Input ] 
          │
          ▼
┌──────────────────┐
│   FastAPI REST   │
└─────────┬────────┘
          │
          ▼
┌──────────────────┐      High Risk?      ┌───────────────────────┐
│  XGBoost Model   │ ───────────────────► │  OpenAI Retention AI  │
└─────────┬────────┘    (Probability > 0.5) └───────────┬───────────┘
          │                                             │
          │ Low Risk                                    │ Generates Offer
          ▼                                             ▼
┌───────────────────────────────────────────────────────────────────┐
│                      JSON Response Output                         │
└───────────────────────────────────────────────────────────────────┘
```

---

## 🔌 Example API Usage

### Endpoint: `POST /predict-with-retention`

#### Request Payload:
```json
{
  "actual_delivery_days": 35.0,
  "delivery_diff_days": 15.0,
  "is_delayed": 1,
  "items_count": 1,
  "total_order_value": 45.0,
  "total_freight_value": 35.0,
  "avg_product_weight": 200.0,
  "avg_photos_qty": 1.0,
  "avg_description_length": 100.0
}
```

#### Response (200 OK):
```json
{
  "churn_probability": 0.8035,
  "is_high_risk": true,
  "retention_strategy": "Drogi Kliencie, rozumiemy, jak frustrujące mogą być długie oczekiwania na zamówienie, i chcemy serdecznie przeprosić za opóźnienie w dostawie. W ramach rekompensaty oferujemy 20% zniżki na Twoje następne zakupy...",
  "status": "success"
}
```

---

## 🌟 Key Business Impact & Results

* **End-to-End Automation**: Zero human intervention required from prediction to retention action dispatch.
* **Cost Efficiency**: LLM execution is conditionally triggered only for high-risk customers (`is_high_risk: true`), significantly optimizing API token costs.
* **Production Reliability**: Containerized environment backed by automated CI/CD pipelines guarantees seamless, bug-free deployments to cloud infrastructure.