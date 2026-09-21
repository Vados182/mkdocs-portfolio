# 📊 TikTok Analytics & AI Sentiment Agent

An end-to-end automated system designed to ingest, analyze sentiment, and summarize TikTok video text using Generative AI, connected to a real-time interactive analytical dashboard.

**2026-09-16**

---

## 🔗 Quick Links
* **Live Dashboard:** [tiktok-ai-analytics.onrender.com](https://tiktok-ai-analytics.onrender.com)
* **GitHub Repository:** [GitHub Link](https://github.com/Vados182/Tiktok-ai-analytics)

---

## 🚀 Project Overview

This project addresses the challenge of manually analyzing large volumes of unstructured social media text data. The system automatically fetches unanalyzed posts from a PostgreSQL database, processes them through Google's Gemini AI model for emotional classification and concise summarization, and visualizes the results on an interactive Streamlit dashboard.

### Key Features:
* **AI Sentiment Analysis:** Automatically classifies post content into *Positive*, *Neutral*, or *Negative* sentiment.
* **Text Summarization:** Generates single-sentence summaries covering the core message of each video script.
* **CI/CD Automation:** Scheduled background processing via GitHub Actions without requiring local server execution.
* **Interactive Dashboard:** Displays real-time sentiment distribution charts and post popularity rankings with dynamic filtering.

---

## 🛠️ Tech Stack

* **Language:** Python 3.11+
* **AI Model:** Google Gemini API (`gemini-3.6-flash`)
* **Database:** PostgreSQL (hosted on Render)
* **Visualization:** Streamlit, Pandas, Plotly Express
* **Automation / CI/CD:** GitHub Actions (Scheduled Cron Workflows)