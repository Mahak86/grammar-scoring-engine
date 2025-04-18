# grammar-scoring-engine
A simple yet powerful engine that transcribes voice samples to text and evaluates the grammar quality of the transcription.
# 📝 Grammar Scoring Engine for Voice Samples

This project provides a simple yet effective pipeline for trancribing voice recordings into text and evaluating the grammar quality of the transcription using both rule-based and AI-powered models.

## 🚀 Features

- 🔊 Transcribes speech to text using [OpenAI Whisper](https://github.com/openai/whisper)
- 🧠 Checks grammar issues using:
  - `language-tool-python` (rule-based)
  - HuggingFace's `vennify/t5-base-grammar-correction` model (AI-based)
- 📊 Computes a grammar similarity score to quantify how "clean" the original text is

---

## 📦 Requirements

You can install all dependencies with:

```bash
pip install -q openai-whisper
pip install -q language-tool-python
pip install transformers


💻 How to Use
Upload a voice sample (e.g., .mp3, .wav)

Transcribe the audio to text using Whisper

Analyze grammar using:

language_tool_python (rule-based)

T5 model via Hugging Face (AI-based)

Compare the original vs corrected text and generate a grammar score

📈 Grammar Score
A similarity metric compares the original and corrected text to produce a percentage score. A higher score means better grammar in the original transcription.


👨‍💻 Author
Your Name – @Mahak86
