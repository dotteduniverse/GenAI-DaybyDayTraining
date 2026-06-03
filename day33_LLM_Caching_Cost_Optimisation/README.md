# Day 33: LLM Caching & Cost Optimisation

## Learning Goals
- Understand the benefits of caching LLM responses to reduce cost and latency.
- Differentiate between exact‑match caching and semantic caching.
- Implement a semantic cache using Redis + embeddings (FAISS or Redis Stack).

## Topics Covered
1. Exact‑match caching (simple dictionary).
2. Semantic caching: store embeddings of queries, retrieve similar cached responses.
3. Using Redis with the `redisvl` or `redis‑py` and vector search.
4. Cost‑saving strategies (TTL, similarity thresholds, cache warming).

## Setup
```bash
pip install redis redisvl openai numpy