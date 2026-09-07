# 🏠 Kalkulator Cen Mieszkań w Warszawie

**2026-08-14**

[![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://kalkulator-mieszkan-warszawa-mwvogqtaov9nyf7h6fsmaj.streamlit.app)
[![GitHub](https://img.shields.io/badge/GitHub-Repository-181717?logo=github)](https://github.com/Vados182/kalkulator-mieszkan-warszawa)

Aplikacja webowa end-to-end do szacowania wartości nieruchomości na rynku warszawskim. Projekt łączy tradycyjne uczenie maszynowe (Machine Learning) z technologiami GenAI, umożliwiając wycenę mieszkania na podstawie formularza lub surowego opisu ogłoszenia.

---

## 🚀 Live Demo

Aplikację możesz wypróbować bezpośrednio poniżej lub otworzyć w [nowym oknie](https://kalkulator-mieszkan-warszawa-mwvogqtaov9nyf7h6fsmaj.streamlit.app):

<iframe
  src="https://kalkulator-mieszkan-warszawa-mwvogqtaov9nyf7h6fsmaj.streamlit.app/?embed=true"
  height="750"
  style="width:100%; border:none; border-radius: 12px; box-shadow: 0 4px 12px rgba(0,0,0,0.15);"
></iframe>

---

## 🛠️ Stos Technologiczny & Architektura

* **Machine Learning:** `PyCaret` (selekcja i trenowanie modelu regresyjnego), `scikit-learn`, `pandas`.
* **Generative AI & NLP:** `OpenAI API (gpt-4o-mini)`, `Instructor` (pobieranie ustrukturyzowanych danych z surowego tekstu ogłoszenia).
* **Observability:** `Langfuse` (monitoring wywołań LLM, śledzenie kosztów i opóźnień).
* **User Interface:** `Streamlit` z dedykowanymi stylowaniami CSS.
* **Deployment & CI/CD:** `Git`, `GitHub`, `Streamlit Community Cloud`.

---

## 💡 Kluczowe Funkcjonalności

1. **Szybka Wycena (Formularz):** Pozwala użytkownikowi ręcznie wybrać dzielnicę, metraż, liczbę pokoi oraz piętro, zwracając estymowaną cenę całkowitą oraz cenę za $m^2$.
2. **Analiza Tekstu Ogłoszenia (LLM):** Wklejenie dowolnego opisu mieszkania powoduje automatyczne wyciągnięcie kluczowych parametrów przez model językowy i przekazanie ich do modelu ML.
3. **Observability LLM:** Wszystkie zapytania przetwarzane przez model OpenAI są rejestrowane w panelu Langfuse w celu kontroli jakości i kosztów.