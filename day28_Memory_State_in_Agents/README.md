# Day 28: Memory & State in Agents

## Learning Goals
- Understand the need for memory in conversational agents.
- Implement short‑term memory (conversation buffer) and long‑term memory (vector store with semantic retrieval).
- Integrate both memory types into a ReAct or LangGraph agent.

## Topics Covered
1. Short‑term memory: storing recent messages.
2. Long‑term memory: embedding user facts and retrieving relevant context.
3. Combining memories to personalise agent responses.

## Setup
```bash
pip install langchain-openai faiss-cpu