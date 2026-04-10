# Day 13 – Exercises

1. **Precision comparison** – Create a small test set of 5 queries with known relevant documents. Compute recall@5 for naive, multi‑query, and HyDE.
2. **HyDE variations** – Generate hypothetical documents of different lengths (20, 100, 300 words) and see which works best.
3. **Cohere Rerank** – Sign up for free Cohere API, use `co.rerank()` and compare with local cross‑encoder.
4. **Sub‑query decomposition** – Write a function that breaks a complex question into sub‑queries, retrieves for each, and then asks the LLM to synthesise an answer.