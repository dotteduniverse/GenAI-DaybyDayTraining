# Exercises – Day 32

1. **Add error handling**  
   Modify the streaming endpoint to catch API errors and send a custom error event.

2. **Stop generation**  
   Implement an abort mechanism (e.g., using `asyncio.Task.cancel()`) so the client can stop streaming mid‑response.

3. **Support multiple users**  
   In the FastAPI app, use a dictionary to store active streams per session ID. Allow cancelling a specific user’s stream.

4. **Use Server‑Sent Events library**  
   Replace raw StreamingResponse with `sse-starlette` for cleaner SSE implementation.

5. **Bonus: Streaming from local model**  
   Use a local LLM (e.g., via Ollama) and stream its output similarly. Compare latency.