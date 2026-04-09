
---

## Day 9 – Working with Embeddings – Semantic Search

### `day09_semantic_search/README.md`

```markdown
# Day 9 – Embeddings for Semantic Search

## 🎯 Learning Objectives
- Understand how to use embeddings for information retrieval.
- Build a simple semantic search engine over a document corpus.
- Use FAISS for efficient similarity search.

## 📚 Detailed Concepts

### Semantic search vs. keyword search
- **Keyword search** (e.g., grep, SQL LIKE) finds exact words. Misses synonyms or paraphrases.
- **Semantic search** uses embeddings to find documents that are **conceptually similar** to the query, even if they share no keywords.

### How semantic search works
1. Convert every document in the corpus into an embedding vector (using a sentence‑transformer model).
2. Store these vectors in an index (FAISS, Annoy, or just a NumPy array).
3. Convert the user’s query into an embedding vector.
4. Compute similarity (e.g., cosine similarity) between the query embedding and all document embeddings.
5. Return the top‑k most similar documents.

### FAISS (Facebook AI Similarity Search)
- Library for efficient nearest neighbour search.
- Can handle millions of vectors on a single CPU.
- Index types:
  - `IndexFlatL2`: exact brute‑force L2 distance (slow but accurate for small datasets).
  - `IndexIVFFlat`: approximate, faster for large datasets.

### Choosing an embedding model
- `all-MiniLM-L6-v2` (384 dims): fast, good for English, 80 MB.
- `intfloat/e5-small-v2` (384 dims): better quality, but slower.
- `text-embedding-ada-002` (OpenAI, 1536 dims): state‑of‑the‑art, but paid.

## 🛠️ Setup
```bash
pip install sentence-transformers faiss-cpu