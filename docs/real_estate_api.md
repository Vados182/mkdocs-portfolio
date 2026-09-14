# Warsaw Real Estate Price Predictor (REST API & LLM Observability)

**2026-09-14**

An end-to-end production-grade REST API designed to estimate property prices in Warsaw. The system combines traditional machine learning for valuation with OpenAI GPT-4o-mini for structured feature extraction from raw Polish listings, fully monitored via Langfuse telemetry.

---

## 🔗 Quick Links & Live Demo

- **Interactive API Documentation (Swagger UI):** [https://warsaw-real-estate-api.onrender.com/docs](https://warsaw-real-estate-api.onrender.com/docs)
- **GitHub Repository:** [https://github.com/Vados182/Warsaw-real-estate-api.git](https://github.com/Vados182/Warsaw-real-estate-api.git)

---

## 🏗️ Technical Architecture

The application is built around a modern microservice architecture tailored for production reliability:

1. **FastAPI Framework:** Exposes `/predict` (tabular input) and `/predict-from-text` (unstructured listing description) endpoints.
2. **LLM Feature Extraction (OpenAI + Instructor):** Uses `GPT-4o-mini` wrapped with the `Instructor` library and `Pydantic` schemas to deterministically parse raw text descriptions into typed parameters (`district`, `area_sqm`, `rooms`, `floor`).
3. **Machine Learning Pipeline (PyCaret):** Predicts final property valuation using a tuned regression model trained on historical Warsaw real estate data.
4. **Observability & Monitoring (Langfuse):** Real-time tracking of API latency, token consumption, error rates, and costs per request.
5. **Deployment:** Fully containerized with **Docker** and hosted on **Render.com**.

---

## 🚀 Key Features & Highlights

- **Deterministic JSON Output:** Guarantees strict type validation on LLM responses to prevent runtime errors in the ML pipeline.
- **Production Observability:** Full visibility into LLM calls, tracking costs, and system performance via Langfuse.
- **Auto-Generated Docs:** Interactive Swagger UI documentation available out of the box for testing endpoints.

---

## 💻 Tech Stack

- **Core:** Python 3.11, FastAPI, Uvicorn, Pydantic
- **Machine Learning & AI:** PyCaret, OpenAI (GPT-4o-mini), Instructor
- **Observability:** Langfuse
- **DevOps & Hosting:** Docker, Render, Git