# 🎬 AI Video Subtitle Generator

**2026-09-07**

A web application for automatically generating, editing, translating, and burning subtitles into videos, powered by OpenAI models (Whisper & GPT-4).

[![GitHub Repository](https://img.shields.io/badge/GitHub-Source%20Code-blue?style=for-the-badge&logo=github)](https://github.com/Vados182/AI-Video-Subtitle-Generator)
[![Streamlit App](https://img.shields.io/badge/Streamlit-View%20Live-red?style=for-the-badge&logo=streamlit)](https://ai-video-subtitle-generator-cjdtjdjrbdusghdisffsnv.streamlit.app/)

---

## 🚀 About the Project

The application was created to drastically reduce the time needed to produce professional subtitles for video content. It allows users to upload a video, automatically generate an audio transcription, translate it into one of many supported languages, manually edit the text in an interactive editor, and finally download either the `.srt` file or the final video with "hardcoded" subtitles.

---

## 🛠️ Technologies & Architecture Used

The project was designed with a focus on separating logic from the interface (Modular Architecture), which facilitates testing and development.

* **Python (3.11)** – Main development environment.
* **Streamlit** – Framework for rapid web interface development.
* **OpenAI API** – Integration with Whisper (v3) and GPT-4 models.
* **Pydub** – Python library for audio file manipulation.
* **FFmpeg** – External system tool for advanced conversion and hardcoding subtitles.
* **Git** – Version control system.

---

## 💻 App Preview (Live Demo)

You can test the running application directly in the frame below or open it in a new tab:

<a href="https://subtitle-generator-app-o7rksymdduw2aydy3q6p4e.streamlit.app/" target="_blank">
  <button style="background-color: #ff4b4b; color: white; padding: 12px 24px; border: none; border-radius: 6px; cursor: pointer; font-size: 16px; font-weight: bold; box-shadow: 0 2px 5px rgba(0,0,0,0.2);">
    🚀 Open Live Demo in New Tab
  </button>
</a>