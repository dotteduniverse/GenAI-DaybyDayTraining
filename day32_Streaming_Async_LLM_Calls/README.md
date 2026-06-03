# Day 32: Streaming & Async LLM Calls

## Learning Goals
- Understand how to stream LLM responses token by token.
- Build an asynchronous chat endpoint using FastAPI.
- Create a simple HTML/JavaScript client to display streaming output.

## Topics Covered
1. OpenAI API streaming with `stream=True`.
2. FastAPI `StreamingResponse` for server‑sent events.
3. Building a minimal frontend with fetch + ReadableStream.

## Setup
```bash
pip install fastapi uvicorn openai sse-starlette