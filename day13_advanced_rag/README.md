# Day 13 – Advanced RAG: Query Transformations & Reranking

## 🎯 Learning Objectives
- Understand limitations of naive RAG (single query, fixed retrieval).
- Implement query transformations: multi‑query, HyDE (Hypothetical Document Embeddings).
- Use a reranker to improve retrieval precision.

## 📚 Detailed Concepts

### Why advanced RAG?
Naive RAG retrieves documents using the raw user query. Problems:
- Short or ambiguous queries retrieve poor results.
- Lexical mismatch (different wording).
- Retrieval might bring irrelevant documents.

### Query transformation techniques
1. **Multi‑query**: Generate multiple rephrased versions of the query, retrieve for each, combine results.
2. **HyDE (Hypothetical Document Embeddings)**: Ask the LLM to generate a hypothetical answer (or document) and use **that** as the retrieval query. Works surprisingly well.
3. **Sub‑queries**: Break a complex question into simpler sub‑questions, retrieve for each, then aggregate.

### Reranking
After retrieving top‑k documents (e.g., 20), use a more powerful **cross‑encoder** model to re‑score them and pick the top‑n (e.g., 5).  
Cross‑encoders are slower but more accurate than bi‑encoders (used for initial retrieval).

### Popular rerankers
- `cross-encoder/ms-marco-MiniLM-L-6-v2` (fast, decent).
- `BAAI/bge-reranker-base` (strong).
- Cohere Rerank API (paid).

## 🛠️ Setup
```bash
pip install langchain chromadb openai sentence-transformers