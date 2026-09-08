# 🏠 Warsaw Real Estate Price Calculator

**2026-08-14**

[![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://kalkulator-mieszkan-warszawa-mwvogqtaov9nyf7h6fsmaj.streamlit.app)
[![GitHub](https://img.shields.io/badge/GitHub-Repository-181717?logo=github)](https://github.com/Vados182/kalkulator-mieszkan-warszawa)

An end-to-end web application for estimating property values in the Warsaw market. The project combines traditional Machine Learning with GenAI technologies, enabling property valuation based on a form or a raw listing description.

---

## 🚀 Live Demo

You can try the app directly below or open it in a [new window](https://kalkulator-mieszkan-warszawa-mwvogqtaov9nyf7h6fsmaj.streamlit.app):

<iframe
  src="https://kalkulator-mieszkan-warszawa-mwvogqtaov9nyf7h6fsmaj.streamlit.app/?embed=true"
  height="750"
  style="width:100%; border:none; border-radius: 12px; box-shadow: 0 4px 12px rgba(0,0,0,0.15);"
></iframe>

---

## 🛠️ Tech Stack & Architecture

* **Machine Learning:** `PyCaret` (regression model selection and training), `scikit-learn`, `pandas`.
* **Generative AI & NLP:** `OpenAI API (gpt-4o-mini)`, `Instructor` (extracting structured data from raw listing text).
* **Observability:** `Langfuse` (LLM call monitoring, cost tracking, and latency monitoring).
* **User Interface:** `Streamlit` with custom CSS styling.
* **Deployment & CI/CD:** `Git`, `GitHub`, `Streamlit Community Cloud`.

---

## 💡 Key Features

1. **Quick Valuation (Form):** Allows the user to manually select the district, area size, number of rooms, and floor, returning the estimated total price and price per $m^2$.
2. **Listing Text Analysis (LLM):** Pasting any apartment description automatically extracts key parameters via a language model and passes them to the ML model.
3. **LLM Observability:** All queries processed by the OpenAI model are logged in the Langfuse dashboard for quality and cost control.