# Day 3 – Tokenization & Embeddings

## 🎯 Learning Objectives
- Understand what tokens are and how text is split before feeding into an LLM.
- Learn about different tokenization algorithms (BPE, WordPiece, SentencePiece).
- Visualise tokenisation using `tiktoken` (OpenAI) and Hugging Face tokenizers.
- Understand embeddings – dense vector representations of words/sentences.
- Compute and compare embeddings using a small model (e.g., `all-MiniLM-L6-v2`).

## 📚 Concepts Covered
- Byte‑pair encoding (BPE) and subword tokens.
- Why tokenisation matters for cost, context length, and multilingual support.
- Embeddings as numeric vectors that capture semantic meaning.
- Cosine similarity between embeddings.

## 🛠️ Setup
Install required packages:

```bash
pip install tiktoken transformers sentence-transformers scikit-learn matplotlib