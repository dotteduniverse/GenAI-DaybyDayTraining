# Day 31: Prompt Injection & Defences

## Learning Goals
- Understand prompt injection attacks (direct and indirect).
- Implement a basic prompt injection detector using heuristics and LLM classification.
- Apply defence techniques: input sanitisation, instruction separation, and filtering.

## Topics Covered
1. Types of prompt injection (e.g., "ignore previous instructions").
2. Building a detector that flags suspicious patterns.
3. Using an LLM judge to classify user inputs as injection attempts.
4. Mitigation strategies (delimiters, random sequence insertion, etc.).

## Setup
```bash
pip install openai