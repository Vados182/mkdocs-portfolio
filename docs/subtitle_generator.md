# 🎬 AI Video Subtitle Generator

Aplikacja webowa do automatycznego generowania, edycji, tłumaczenia i wtapiania napisów do filmów, oparta na modelach OpenAI (Whisper & GPT-4).

[![GitHub Repository](https://img.shields.io/badge/GitHub-Kod%20źródłowy-blue?style=for-the-badge&logo=github)](https://github.com/twoja-nazwa-uzytkownika/nazwa-repozytorium)
[![Streamlit App](https://img.shields.io/badge/Streamlit-Zobacz%20Live-red?style=for-the-badge&logo=streamlit)](https://subtitle-generator-app-o7rkxymdduw2aydy3q6p4e.streamlit.app)

---

## 🚀 O Projekcie

Aplikacja została stworzona, aby drastycznie skrócić czas potrzebny na tworzenie profesjonalnych napisów do materiałów wideo. Pozwala użytkownikom wgrać film, automatycznie wygenerować transkrypcję audio, przetłumaczyć ją na jeden z wielu obsługiwanych języków, ręcznie edytować tekst w interaktywnym edytorze i ostatecznie pobrać sam plik `.srt` lub gotowy film z wtopionymi ("hardcoded") napisami.

---

## 🛠️ Użyte Technologie & Architektura

Projekt został zaprojektowany z dbałością o separację logiki od interfejsu (Modular Architecture), co ułatwia testowanie i rozwój.

* **Python (3.11)** – Główne środowisko programistyczne.
* **Streamlit** – Framework do szybkiego tworzenia interfejsów webowych.
* **OpenAI API** – Integracja z modelami Whisper (v3) i GPT-4.
* **Pydub** – Biblioteka do manipulacji plikami audio.
* **FFmpeg** – Zewnętrzne narzędzie systemowe do zaawansowanej konwersji i wtapiania napisów.
* **Git** – System kontroli wersji.

---

## 💻 Podgląd Aplikacji (Live Demo)

Możesz przetestować działającą aplikację bezpośrednio w ramce poniżej lub przejść do niej w nowej karcie:

<div style="position: relative; width: 100%; height: 700px; overflow: hidden; border-radius: 8px; border: 1px solid #333;">
  <iframe src="https://subtitle-generator-app-o7rkxymdduw2aydy3q6p4e.streamlit.app/?embed=true" 
          style="width: 100%; height: 100%; border: none;" 
          allow="accelerometer; ambient-light-sensor; camera; encrypted-media; geolocation; gyroscope; hid; microphone; midi; payment; usb; vr; xr-spatial-tracking" 
          sandbox="allow-forms allow-modals allow-popups allow-presentation allow-same-origin allow-scripts">
  </iframe>
</div>