# Day 29: LLM as a Judge – Evaluation & Guardrails

## Learning Goals
- Understand the concept of using an LLM to evaluate and moderate content.
- Build a content moderation agent that classifies text as safe/unsafe.
- Implement guardrails to filter harmful or off‑topic queries.

## Topics Covered
1. Using an LLM as a binary or multi‑class classifier.
2. Creating a moderation prompt with detailed rubrics.
3. Integrating the judge into a guardrail before main agent execution.

## Setup
```bash
pip install openai