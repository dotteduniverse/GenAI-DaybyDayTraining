# Day 30: Fine‑tuning with RLHF (Conceptual)

## Learning Goals
- Understand the RLHF pipeline: Supervised Fine‑Tuning (SFT) → Reward Modelling → Reinforcement Learning (PPO).
- Use TRL (Transformer Reinforcement Learning) to fine‑tune a reward model on a preference dataset.
- Conceptually grasp how human preferences are used to align LLMs.

## Topics Covered
1. Loading a preference dataset (e.g., Anthropic HH‑RLHF).
2. Training a reward model with TRL’s `RewardTrainer`.
3. (Optional) Using the reward model for PPO fine‑tuning.

## Setup
```bash
pip install trl transformers datasets torch accelerate peft