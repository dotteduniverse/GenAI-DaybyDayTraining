## Day 10 – Mini Project: Multi‑turn Conversational Agent

### `day10_conversational_agent/README.md`

```markdown
# Day 10 – Mini Project: Conversational Agent with Memory

## 🎯 Learning Objectives
- Combine LLM API calls with conversation memory.
- Implement a chatbot that remembers previous exchanges.
- Add a simple persona or system prompt.
- Handle token limits by trimming history.

## 📚 Detailed Concepts

### Conversation memory
- To have a multi‑turn conversation, you must send the entire history each time.
- The API is stateless – it does not remember past calls.
- Store messages in a Python list:
  ```python
  messages = [
      {"role": "system", "content": "You are a helpful assistant."},
      {"role": "user", "content": "What is AI?"},
      {"role": "assistant", "content": "AI is ..."},
      {"role": "user", "content": "Tell me more."}
  ]

## 📝 Exercises
- Add a `!save` command that writes the conversation to a file.
- Implement a token counter; when total tokens exceed 3000, remove the oldest exchange.
- Change the persona to “a pirate” and test.

## ✅ Checkpoint
You have a fully functional conversational agent.