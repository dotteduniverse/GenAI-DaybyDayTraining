# Day 40: Mini Project – Multi‑Agent Debate System

## Learning Goals
- Understand how multi‑agent debates can improve answer quality.
- Build a system where two agents with different personas debate a question.
- Implement a judge agent to evaluate arguments and produce a final refined answer.

## Project Overview
You will create:
1. **Agent A** (e.g., optimistic / creative)
2. **Agent B** (e.g., critical / analytical)
3. **Judge** (evaluates the debate and synthesises a final answer)

The agents debate a given prompt over several rounds, then the judge outputs a refined, more accurate response.

## Topics Covered
1. Multi‑agent conversation loop.
2. Persona‑based prompting.
3. Debate termination conditions (e.g., max rounds, convergence).
4. Final synthesis with judge.

## Setup
```bash
pip install openai