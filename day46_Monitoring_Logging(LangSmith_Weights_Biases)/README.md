# Day 46: Monitoring & Logging (LangSmith, Weights & Biases)

## Learning Goals
- Understand the importance of monitoring LLM applications: tracing, latency, cost, quality.
- Set up LangSmith to trace and debug chains/agents.
- (Optional) Use Weights & Biases (wandb) for logging metrics and visualisations.

## Topics Covered
1. LangSmith: tracing, feedback, run visualisation, and dataset evaluation.
2. Adding LangSmith callbacks to LangChain applications.
3. Wandb: logging prompts, responses, metrics, and custom charts.
4. Integrating monitoring into your deployed capstone.

## Setup
```bash
pip install langsmith wandb