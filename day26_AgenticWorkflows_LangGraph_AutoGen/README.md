# Day 26: Agentic Workflows – LangGraph / AutoGen

## Learning Goals
- Understand the concept of agentic workflows (tools, reasoning, execution).
- Build a simple agent that can use tools: calculator + web search.
- Use LangGraph to define a graph of agent steps.

## Topics Covered
1. Defining tools (calculator, search) for an LLM.
2. Building a ReAct‑style agent with LangGraph.
3. Executing agent loop with tool calling.

## Setup
```bash
pip install langgraph langchain langchain-openai tavily-python