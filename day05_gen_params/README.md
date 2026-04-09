# Day 5 – Text Generation Parameters

## 🎯 Learning Objectives
- Understand how generation parameters control output.
- Experiment with temperature, top‑k, top‑p, repetition penalty.
- Build an interactive text generator with sliders.

## 📚 Concepts Covered
- Temperature scaling of logits.
- Top‑k sampling: restrict to k most likely tokens.
- Top‑p (nucleus) sampling: cumulative probability threshold.
- Repetition penalty to avoid loops.

## 🛠️ Setup
```bash
pip install transformers gradio