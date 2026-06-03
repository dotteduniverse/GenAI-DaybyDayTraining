# Exercises – Day 47

1. **Add API key to your deployed Space**  
   In your HF Space, set an environment variable `API_KEY`. Modify `app.py` to check for this key in the request headers (for Gradio, use `gr.Request`). Test with correct and incorrect keys.

2. **Implement user‑specific limits**  
   Extend the FastAPI code to support multiple API keys, each with its own rate limit (e.g., `free: 10/hour`, `pro: 1000/hour`). Store keys and limits in a JSON file.

3. **Log failed attempts**  
   Add logging (to file or console) whenever an invalid API key is used or a rate limit is exceeded. Include timestamp and IP address.

4. **Add a `GET /status` endpoint**  
   Return the remaining rate limit for the current API key (requires storing usage counters). Use a Redis or in‑memory dictionary.

5. **Bonus: JWT authentication**  
   Replace simple API key with JWT (JSON Web Token). Implement a `/login` endpoint that returns a token, and protect `/generate` with `HTTPBearer`.