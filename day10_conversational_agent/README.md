# Day 10 – Mini Project: Conversational Agent with Memory

## 🎯 Learning Objectives
- Combine LLM API calls with conversation memory.
- Implement a chatbot that remembers previous exchanges.
- Add a simple persona or system prompt.

## 📚 Concepts Covered
- Maintaining message history.
- Handling long conversations (trimming or summarising).
- Basic prompt engineering for consistent persona.

## 🚀 Step‑by‑Step Tasks
1. Use OpenAI (or Cohere) to create a chatbot loop.
2. Store messages in a list and send full history each turn.
3. Set a system message: *“You are a helpful and friendly assistant.”*
4. Extend with a simple command to clear memory.

## 📝 Exercises
- Add a `!save` command that writes the conversation to a file.
- Implement a token counter; when total tokens exceed 3000, remove the oldest exchange.
- Change the persona to “a pirate” and test.

## ✅ Checkpoint
You have a fully functional conversational agent.