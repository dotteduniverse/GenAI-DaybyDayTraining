# 🧠 50 Days of Generative AI – A Structured Learning Journey

Welcome to **genai-50-days** – a hands‑on, code‑first curriculum to master Generative AI from fundamentals to advanced applications.  
Whether you're a developer, data scientist, or AI enthusiast, this repo will guide you through 50 days of practical projects, theory, and industry‑relevant tools.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
![Python 3.10+](https://img.shields.io/badge/python-3.10%2B-blue)
![OpenAI](https://img.shields.io/badge/OpenAI-API-412991)
![Hugging Face](https://img.shields.io/badge/🤗%20Hugging%20Face-Transformers-ffd21e)

---

## 📚 Table of Contents
- [What You Will Learn](#what-you-will-learn)
- [Prerequisites](#prerequisites)
- [Repository Structure](#repository-structure)
- [Step‑by‑Step Guide for Learners](#step‑by‑step-guide-for-learners)
  - [Phase 1: Foundations (Days 1–10)](#phase-1-foundations-days-1-10)
  - [Phase 2: Core Techniques (Days 11–25)](#phase-2-core-techniques-days-11-25)
  - [Phase 3: Advanced & Applied GenAI (Days 26–40)](#phase-3-advanced--applied-genai-days-26-40)
  - [Phase 4: Project & Deployment (Days 41–50)](#phase-4-project--deployment-days-41-50)
- [How to Use This Repository](#how-to-use-this-repository)
- [Recommended Resources](#recommended-resources)
- [Contributing & Feedback](#contributing--feedback)
- [License](#license)

---

## 🎯 What You Will Learn
- **Generative AI fundamentals** – language models, diffusion, GANs, VAEs
- **Prompt engineering** for LLMs (GPT, Llama, Claude)
- **Fine‑tuning** and **RAG** (Retrieval‑Augmented Generation)
- **Multimodal generation** (text + images) with Stable Diffusion, DALL‑E, CLIP
- **Agentic workflows** – LangChain, function calling, tool use
- **Deployment** – APIs, streaming, cost optimisation, evaluation

Each day includes a mix of theory, code notebooks, and small projects.

---

## ✅ Prerequisites
- **Python 3.10+** – comfortable with functions, classes, and Jupyter notebooks
- **Basic machine learning** – knows what training/validation means
- **Command line** – installing packages, running scripts
- A **Hugging Face** account (free) and an **OpenAI API key** (budget ~$10)

> No deep learning PhD required – we’ll explain concepts as we go!

---

## 📁 Repository Structure
genai-50-days/
├── day01_intro/
├── day02_prompt_basics/
├── ...
├── day50_final_project/
├── resources/ # Cheat sheets, papers, links
├── requirements.txt
├── .env.example
└── README.md

Each day’s folder contains:
- `README.md` – learning objectives & instructions
- `notebook.ipynb` – interactive code
- `exercises/` – optional challenges
- `solutions/` – (available after day’s end)

---

## 👣 Step‑by‑Step Guide for Learners

### Phase 1: Foundations (Days 1–10)
Build your GenAI toolkit and understand core concepts.

| Day | Topic | Hands‑on Task |
|-----|-------|----------------|
| 1   | What is Generative AI? – History & use cases | Explore famous models (GPT, Stable Diffusion) |
| 2   | Prompt engineering basics | Write 10 prompts for ChatGPT, compare outputs |
| 3   | Tokenization & embeddings | Visualise tokens with `tiktoken` |
| 4   | Intro to Hugging Face `transformers` | Load & run a small GPT‑2 model |
| 5   | Text generation parameters (temperature, top‑p, etc.) | Build an interactive text generator |
| 6   | LLM APIs – OpenAI & Cohere | Create a simple Q&A bot |
| 7   | Ethics & bias in GenAI | Red‑team a prompt, discuss safeguards |
| 8   | Intro to image generation (Diffusion models) | Generate an image with Stable Diffusion (free colab) |
| 9   | Working with embeddings – semantic search | Build a document search engine |
| 10  | **Mini project:** Multi‑turn conversational agent | Combine LLM API + memory |

### Phase 2: Core Techniques (Days 11–25)
Dive deeper into fine‑tuning, RAG, and controlling outputs.

| Day | Topic | Hands‑on Task |
|-----|-------|----------------|
| 11  | Fine‑tuning with LoRA (using PEFT) | Fine‑tune a small LLM on your own data |
| 12  | Retrieval‑Augmented Generation (RAG) basics | Use LangChain + ChromaDB |
| 13  | Advanced RAG – query transformations & reranking | Improve retrieval quality |
| 14  | Prompt chaining & self‑consistency | Build a multi‑step reasoning chain |
| 15  | Structured output – JSON mode & function calling | Extract info from messy text |
| 16  | Evaluating LLMs (BLEU, ROUGE, custom metrics) | Create an evaluation harness |
| 17  | Working with local models (Llama 3, Mistral) | Run llama.cpp or Ollama |
| 18  | Quantisation – GGUF, GPTQ | Load a 4‑bit model on a laptop |
| 19  | Prompt optimisation – AutoPrompt, DSPy | Use DSPy to optimise a prompt |
| 20  | **Mini project:** RAG chatbot for a PDF collection | Build & evaluate a Q&A system |
| 21  | Intro to multimodal – CLIP & BLIP | Image‑to‑text & zero‑shot classification |
| 22  | Text‑to‑image with control (ControlNet, IP‑Adapter) | Condition generation on sketches |
| 23  | Image‑to‑image & inpainting | Use Diffusers to edit an image |
| 24  | Video generation basics (Stable Video Diffusion) | Create a short looping animation |
| 25  | **Mini project:** Multimodal search engine (text + image) | Combine CLIP + FAISS |

### Phase 3: Advanced & Applied GenAI (Days 26–40)
Agents, LLM ops, and advanced architectures.

| Day | Topic | Hands‑on Task |
|-----|-------|----------------|
| 26  | Agentic workflows – LangGraph / AutoGen | Build a tool‑using agent (calculator + search) |
| 27  | ReAct prompting & reasoning | Implement a ReAct agent from scratch |
| 28  | Memory & state in agents | Add short‑term & long‑term memory |
| 29  | LLM as a judge – evaluation & guardrails | Create a content moderation agent |
| 30  | Fine‑tuning with RLHF (conceptual) | Use TRL to fine‑tune a reward model |
| 31  | Prompt injection & defences | Build a basic prompt injection detector |
| 32  | Streaming & async LLM calls | Build a real‑time chat interface (FastAPI) |
| 33  | LLM caching & cost optimisation | Implement semantic caching (Redis + embeddings) |
| 34  | Working with very long context (100k+) | Summarise a full book using map‑reduce |
| 35  | **Mini project:** Autonomous research assistant | Agent that searches, reads, and summarises |
| 36  | Diffusion model fine‑tuning (DreamBooth) | Fine‑tune Stable Diffusion on your face |
| 37  | Text‑to‑3D & NeRF basics | Generate a 3D object with Shap‑E |
| 38  | Music & audio generation (AudioLDM 2) | Create a short melody from a prompt |
| 39  | Model merging & weight interpolation | Merge two LLMs with mergekit |
| 40  | **Mini project:** Multi‑agent debate system | Two agents argue & refine answers |

### Phase 4: Project & Deployment (Days 41–50)
Build a portfolio‑ready application and learn deployment.

| Day | Topic | Hands‑on Task |
|-----|-------|----------------|
| 41  | Project ideation & design doc | Choose your capstone project (chatbot, art tool, etc.) |
| 42  | Data collection & preprocessing | Create a dataset for your project |
| 43  | Prototype with Gradio / Streamlit | Build an interactive UI |
| 44  | Optimisation – faster inference (vLLM, TGI) | Deploy model with vLLM |
| 45  | API deployment (Replicate, Hugging Face Spaces) | Push your app to a public endpoint |
| 46  | Monitoring & logging (LangSmith, Weights & Biases) | Add trace logging |
| 47  | Security & rate limiting | Protect your API with API keys |
| 48  | Writing a technical blog post | Document your project |
| 49  | Final polish & testing | User testing & bug fixes |
| 50  | **Project showcase & presentation** | Record a demo video & submit |

---

## 🚀 How to Use This Repository

1. **Clone the repo**  
   ```bash
   git clone https://github.com/dotteduniverse/GenAI-DaybyDayTraining.git
   cd GenAI-DaybyDayTraining
