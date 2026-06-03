# Exercises – Day 33

1. **Benchmark cache hit rate**  
   Use 20 diverse queries. Run them twice: first to populate cache, second with semantically similar paraphrases (e.g., “What’s the weather like?” → “Tell me the current weather”). Measure hit rate.

2. **Adjust similarity threshold**  
   Vary the threshold from 0.7 to 0.95. Report how hit rate and accuracy trade off.

3. **Persistent Redis cache**  
   Set up Redis Stack (Docker: `docker run -p 6379:6379 redis/redis-stack-server`). Implement `RedisSemanticCache` using `redisvl` or `redis` + vector search.

4. **Cache warm‑up**  
   Pre‑populate the cache with responses to frequently asked questions (from a log file or common queries). Measure cold‑start latency reduction.

5. **Bonus: Multi‑model caching**  
   Extend the cache to work with multiple models (e.g., `gpt-3.5-turbo` vs `gpt-4`). Use (query, model) as the cache key.