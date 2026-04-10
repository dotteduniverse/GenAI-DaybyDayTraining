# Day 17 – Working with Local Models (Llama 3, Mistral)

## 🎯 Learning Objectives
- Run LLMs locally using Ollama, llama.cpp, or Hugging Face.
- Understand the trade‑offs (privacy, cost, speed, quality).
- Generate text with a 7B model on a laptop.

## 📚 Detailed Concepts

### Why local models?
- **Privacy**: data never leaves your machine.
- **No API costs**.
- **Offline** use.
- **Customisation**: you can fine‑tune and deploy anywhere.

### Challenges
- **Hardware**: 7B model requires ~6‑8 GB RAM/VRAM (quantised).
- **Speed**: slower than API (tokens/second depends on CPU/GPU).
- **Quality**: smaller models (7B) are below GPT‑3.5.

### Popular local models
- **Llama 3 (8B)** – Meta, strong performance.
- **Mistral 7B** – efficient, permissive license.
- **Phi‑3 mini (3.8B)** – runs on phone.

### Tools
- **Ollama** – simplest: `ollama run llama3`.
- **llama.cpp** – optimised for CPU, supports GGUF quantisation.
- **Transformers** – load with `AutoModelForCausalLM`, use 4‑bit quantisation (bitsandbytes).

## 🛠️ Setup
Install Ollama (macOS/Linux/Windows WSL2):  
```bash
curl -fsSL https://ollama.com/install.sh | sh
ollama pull llama3