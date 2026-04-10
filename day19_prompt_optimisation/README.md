# Day 19 – Prompt Optimisation: AutoPrompt, DSPy

## 🎯 Learning Objectives
- Understand automated prompt optimisation.
- Use DSPy to compile and optimise prompts.
- Learn about gradient‑based prompt tuning (AutoPrompt).

## 📚 Detailed Concepts

### Why automate prompt engineering?
Manual prompt tuning is tedious. Automated methods search over prompt variations to maximise performance on a validation set.

### DSPy (Stanford)
- Framework for **programming with foundation models**.
- You write a **signature** (input → output) and a **program** (module composition).
- DSPy optimises prompts and few‑shot examples using **teleprompters** (e.g., BootstrapFewShot, MIPRO).

### AutoPrompt (Shin et al. 2020)
- Gradient‑based search for trigger tokens that maximise a target output.
- Used for eliciting specific behaviours (e.g., sentiment analysis).

### Other methods
- **OPRO** (Optimising Prompts by Reinforcement Learning) – used by Google for prompt optimisation.
- **APO** (Automatic Prompt Optimiser) – uses LLM feedback to refine prompts.

## 🛠️ Setup
```bash
pip install dspy-ai