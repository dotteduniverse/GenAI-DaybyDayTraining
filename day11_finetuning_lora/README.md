# Day 11 – Fine‑tuning with LoRA (Low‑Rank Adaptation)

## 🎯 Learning Objectives
- Understand why fine‑tuning is needed and its challenges (full fine‑tuning is expensive).
- Learn LoRA: a parameter‑efficient fine‑tuning (PEFT) method.
- Fine‑tune a small LLM (e.g., GPT‑2 or Llama‑2‑7b) on a custom dataset using LoRA.
- Evaluate the fine‑tuned model.

## 📚 Detailed Concepts

### Why fine‑tune?
Pre‑trained models are generalists. Fine‑tuning adapts them to a specific domain or task (e.g., medical Q&A, legal document summarisation).  
However, full fine‑tuning updates **all** model parameters, requiring:
- A large GPU (e.g., 80GB for a 7B model).
- Lots of training data.
- Risk of catastrophic forgetting.

### LoRA (Low‑Rank Adaptation) – [Hu et al. 2021](https://arxiv.org/abs/2106.09685)
- Instead of updating the full weight matrix `W`, LoRA injects trainable **low‑rank matrices** `A` and `B` such that `W' = W + BA`.
- `B` has dimensions `(d, r)`, `A` has `(r, k)`, with `r << min(d, k)` (e.g., r=8).
- Only `A` and `B` are trained – a tiny fraction of parameters (often <1%).
- **Advantages**:  
  - Extremely memory efficient (no need to store gradients for frozen weights).  
  - Fast to train.  
  - Multiple LoRA adapters can be swapped without duplicating the base model.

### PEFT library (Hugging Face)
- Provides LoRA, AdaLoRA, Prefix Tuning, etc.
- Works with any `transformers` model.

### Training data format
For text generation, use a simple prompt‑completion format. Example (instruction‑response):