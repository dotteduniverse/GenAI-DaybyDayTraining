# Exercises – Day 44

1. **Run vLLM server**  
   Start the API server with a small model (e.g., `TinyLlama/TinyLlama-1.1B-Chat-v1.0`). Send 5 different prompts via `requests`.

2. **Compare throughput**  
   Generate 20 prompts (same batch) with vLLM offline and with HF pipeline. Measure total time. Compute tokens per second for each.

3. **Change model parameters**  
   Adjust `max_tokens`, `temperature`, `top_p` in the vLLM library call. See how output changes.

4. **Try TGI**  
   Run TGI via Docker (if you have GPU). Send a request and measure latency.

5. **Bonus: Optimise your own project**  
   If your capstone uses an LLM (e.g., for RAG), replace the OpenAI or local HF call with vLLM. Report speed improvement.