# 🎙️ Audex-Lite: Unified Audio Intelligence with OpenRouter

> A research-oriented implementation inspired by the paper **"Unified Audio Intelligence Without Regressing on Text Intelligence"** built using **Google Colab**, **Whisper**, **OpenRouter**, **FAISS**, **PyTorch**, and **Gradio**.

![License](https://img.shields.io/badge/License-MIT-green.svg)
![Python](https://img.shields.io/badge/Python-3.10+-blue.svg)
![Colab](https://img.shields.io/badge/Google-Colab-orange.svg)
![OpenRouter](https://img.shields.io/badge/OpenRouter-API-purple.svg)
![Gradio](https://img.shields.io/badge/Gradio-UI-red.svg)

---

## 📖 Overview

Audex-Lite is an end-to-end multimodal audio intelligence system inspired by the Audex architecture presented in the paper:

> **Unified Audio Intelligence Without Regressing on Text Intelligence**

Instead of reproducing the original 30B unified model, this project implements the **core architectural concepts** using lightweight, open-source components that can run on a **free Google Colab T4 GPU**.

The system combines local audio understanding, cross-modal memory, LLM reasoning, and speech synthesis into a single interactive application.

---

# ✨ Features

* 🎤 Audio upload and microphone recording
* 🗣️ Whisper-based speech recognition
* 🧠 Audio feature extraction using Whisper Encoder
* 🔄 Projection layer for audio embedding alignment
* 💬 OpenRouter-powered reasoning
* 🧠 Cross-modal FAISS memory
* 🤖 Agent-inspired orchestration pipeline
* 🔍 Audio Question Answering
* 😊 Emotion-aware audio analysis
* 🌍 Speech translation
* 📝 Audio summarization
* 🔊 Text-to-Speech response generation
* 📊 Runtime telemetry
* 🌐 Interactive Gradio interface

---

# 🏗️ System Architecture

```text
                User Audio
                     │
                     ▼
           Audio Preprocessing
                     │
                     ▼
            Whisper Encoder
                     │
                     ▼
          Projection Layer
                     │
                     ▼
      Audio Representation Builder
                     │
                     ▼
        Cross-Modal Memory (FAISS)
                     │
                     ▼
      Agentic Prompt Construction
                     │
                     ▼
         OpenRouter Language Model
                     │
                     ▼
          Unified AI Response
                     │
          ┌──────────┴──────────┐
          ▼                     ▼
      Text Output         Speech Output
                     │
                     ▼
                Gradio UI
```

---

# 🚀 Implemented Pipeline

### Phase 1

Environment & Dependency Setup

### Phase 2

Audio Preprocessing

* Audio normalization
* Silence trimming
* Resampling

### Phase 3

Whisper Audio Encoder

* Hidden state extraction
* Speech transcription

### Phase 4

Projection Layer

* Linear projection
* Layer normalization
* Activation
* Embedding alignment

### Phase 5

Audio Representation

Extracts

* Duration
* Energy
* Zero Crossing Rate
* Transcript
* Audio embedding

### Phase 6

Prompt Construction

Builds structured prompts containing

* Acoustic profile
* Semantic transcript
* Memory retrieval
* User instruction

### Phase 7

Unified LLM Reasoning

Uses OpenRouter models for

* Audio understanding
* Question answering
* Summarization
* Translation
* General reasoning

### Phase 8

Cross-Modal Memory

Stores

* Text embeddings
* Audio embeddings

using FAISS.

### Phase 9

Agent-Oriented Reasoning

Implements multiple logical analysis stages

* Acoustic profiling
* Semantic auditing
* Memory retrieval
* Executive reasoning

### Phase 10

Speech Generation

Generates spoken responses using gTTS.

### Phase 11

Interactive Dashboard

Built using Gradio.

---

# 📂 Project Structure

```text
Audex-Lite/

│── notebook.ipynb
│── README.md
│── LICENSE
│── requirements.txt
│── assets/
│── outputs/
```

---

# 🛠️ Technologies Used

* Python
* PyTorch
* Transformers
* Whisper
* OpenRouter API
* FAISS
* Librosa
* NumPy
* SciPy
* Gradio
* gTTS

---

# 🎯 Supported Tasks

* Speech Transcription
* Audio Question Answering
* Speech Translation
* Audio Summarization
* Emotion Analysis
* Conversational Audio Understanding
* Speech Synthesis

---

# 🧠 Cross-Modal Memory

The project maintains two independent vector memories.

### Text Memory

Stores semantic conversation history.

### Audio Memory

Stores Whisper encoder embeddings for acoustic similarity retrieval.

Both memories are indexed using FAISS for efficient nearest-neighbor search.

---

# 📈 Runtime Telemetry

The application reports:

* End-to-end latency
* Memory statistics
* Transcript extraction
* Runtime diagnostics

---

# 💻 Running the Project

## Clone the repository

```bash
git clone https://github.com/yourusername/Audex-Lite.git

cd Audex-Lite
```

## Install dependencies

```bash
pip install -r requirements.txt
```

## Set your OpenRouter API Key

```python
OPENROUTER_API_KEY="your_api_key"
```

## Launch

Run the notebook or execute the Gradio application.

---

# ⚠️ Disclaimer

This repository is **not** an official implementation of the Audex paper.

It is an independent educational and research-oriented implementation inspired by the architectural concepts described in the publication. Several large-scale components from the original work have been replaced with lightweight alternatives suitable for execution on free Google Colab resources.

---

# 🔮 Future Improvements

* Streaming speech processing
* Learnable projection alignment
* Audio token generation
* Neural codec integration
* Speaker diarization
* Long-context memory
* Tool-using voice agents
* Native multimodal decoder
* Benchmark evaluation
* Quantized local LLM support

---

# 🤝 Contributing

Contributions, feature requests, bug reports, and pull requests are welcome.

If you have ideas for improving the architecture or extending the multimodal pipeline, feel free to open an issue or submit a pull request.

---

# 📜 License

This project is licensed under the **MIT License**.

See the `LICENSE` file for details.

---

# 🙏 Acknowledgements

This project builds upon the ideas and open-source work of:

* OpenAI Whisper
* Hugging Face Transformers
* OpenRouter
* FAISS
* PyTorch
* Librosa
* Gradio
* Google Text-to-Speech

Special thanks to the authors of **"Unified Audio Intelligence Without Regressing on Text Intelligence"** for their research and inspiration.
