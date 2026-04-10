
---

## Day 6 – LLM APIs (OpenAI & Cohere) – Simple Q&A Bot

### `day06_llm_apis/README.md`

```markdown
# Day 6 – LLM APIs: OpenAI & Cohere

## 🎯 Learning Objectives
- Use OpenAI’s ChatCompletion API.
- Use Cohere’s generate endpoint.
- Build a simple Q&A bot that answers questions about a given text.

## 📚 Detailed Concepts

### Why use APIs instead of local models?
- **Ease**: no need for GPU or large downloads.
- **Performance**: state‑of‑the‑art models (GPT‑4, Command R+) are much more capable than small local models.
- **Cost**: pay per token – cheap for prototyping.
- **Downside**: requires internet, you don’t own the model, privacy concerns.

### OpenAI API
- **ChatCompletion** endpoint: takes a list of messages, each with `role` (`system`, `user`, `assistant`).
- System message sets the behaviour (e.g., “You are a helpful tutor”).
- Returns a JSON with the assistant’s reply.

### Cohere API
- **Generate** endpoint: simpler – takes a single prompt string.
- Supports `model="command"` or `"command-r"`.
- Also has a chat endpoint similar to OpenAI.

### Prompting for Q&A
- To answer based on a given context, use a prompt like:
- Context: {context}
- Question: {question}
- Answer concisely based only on the context:

### Handling long conversations (memory)
- Store previous messages in a list and send the entire history each time.  
- Be careful of token limits – you may need to truncate older messages.

## 🛠️ Setup
```bash
pip install openai cohere python-dotenv