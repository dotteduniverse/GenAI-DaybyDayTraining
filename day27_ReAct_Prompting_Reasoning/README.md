# Day 27: ReAct Prompting & Reasoning

## Learning Goals
- Understand the ReAct (Reason + Act) paradigm for LLM agents.
- Implement a ReAct agent from scratch without libraries.
- Learn how interleaving reasoning traces and actions improves performance.

## Topics Covered
1. The ReAct loop: Thought → Action → Observation.
2. Implementing a simple agent with tools (calculator, Wikipedia search).
3. Parsing LLM outputs to extract thoughts and actions.

## Setup
```bash
pip install openai wikipedia-api