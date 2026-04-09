
---

## Day 3 – Tokenization & Embeddings

### `day03_tokenization_embeddings/README.md`

```markdown
# Day 3 – Tokenization & Embeddings

## 🎯 Learning Objectives
- Understand what tokens are and how text is split before feeding into an LLM.
- Learn about different tokenization algorithms (BPE, WordPiece, SentencePiece).
- Visualise tokenisation using `tiktoken` (OpenAI) and Hugging Face tokenizers.
- Understand embeddings – dense vector representations of words/sentences.
- Compute and compare embeddings using a small model (e.g., `all-MiniLM-L6-v2`).

## 📚 Detailed Concepts

### Why tokenization?
LLMs do not see raw text; they see numbers (token IDs).  
Tokenization splits text into smaller pieces called **tokens** – typically subwords (e.g., “tokenization” → “token” + “ization”).  
Common algorithms:
- **BPE (Byte‑Pair Encoding)** – used by GPT models. Iteratively merges most frequent byte pairs.
- **WordPiece** – used by BERT. Similar to BPE but merges based on likelihood.
- **SentencePiece** – used by Llama, T5. Treats input as a sequence of Unicode characters.

### Why does tokenization matter?
- **Cost** – OpenAI charges per token (≈0.75 words for English). Longer token sequences cost more.
- **Context length** – A model can only process a fixed number of tokens (e.g., 4096 for GPT-3.5).
- **Multilingual performance** – Some languages (e.g., Japanese) require many more tokens per character.

### What are embeddings?
An embedding is a **dense vector** of floating‑point numbers that represents the **semantic meaning** of a word, sentence, or document.  
- Similar meanings have similar vectors (cosine similarity close to 1).
- They are learned during pre‑training and can be reused.
- Example: `“king”` vector – `“man”` vector + `“woman”` vector ≈ `“queen”` vector.

### Embedding dimensions
- Small: 50‑200 dimensions (fast, less expressive).
- Large: 768‑4096 dimensions (more nuanced, slower).
- We use `all-MiniLM-L6-v2` (384 dimensions) – good balance for learning.

## 🛠️ Setup
```bash
pip install tiktoken transformers sentence-transformers scikit-learn matplotlib