
---

## Day 4 – Intro to Hugging Face Transformers (Load & run GPT‑2)

### `day04_intro_transformers/README.md`

```markdown
# Day 4 – Intro to Hugging Face Transformers

## 🎯 Learning Objectives
- Understand the Hugging Face ecosystem (`transformers`, `datasets`, `pipeline`).
- Load a pre‑trained GPT‑2 model and tokenizer.
- Generate text using the `pipeline` API and low‑level model calls.
- Explore model size and inference speed.

## 📚 Detailed Concepts

### The Hugging Face ecosystem
- **Transformers**: thousands of pre‑trained models (BERT, GPT, T5, Llama, etc.) with a unified API.
- **Datasets**: easy access to hundreds of NLP datasets.
- **Tokenizers**: fast tokenization for all models.
- **Pipeline**: high‑level abstraction for common tasks (text generation, sentiment analysis, etc.).

### Loading a model
Two ways:
1. **Pipeline** (simplest):
   ```python
   generator = pipeline("text-generation", model="gpt2")
   output = generator("Hello", max_length=50)