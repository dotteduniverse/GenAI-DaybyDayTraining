# Day 47: Security & Rate Limiting

## Learning Goals
- Understand common security risks for deployed LLM APIs (abuse, DDoS, excessive usage).
- Add API key authentication to your FastAPI or Gradio app.
- Implement rate limiting (requests per minute per user or IP).

## Topics Covered
1. API key generation and validation (simple token or JWT).
2. Adding `fastapi.Security` with API key header.
3. Rate limiting with `slowapi` (FastAPI) or `gradio` built‑in queue.
4. Storing keys and limits in environment variables or a database.

## Setup
```bash
pip install fastapi uvicorn slowapi python-dotenv