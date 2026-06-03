# Day 36: Diffusion Model Fine‑tuning – DreamBooth

## Learning Goals
- Understand the DreamBooth technique for personalising diffusion models.
- Fine‑tune Stable Diffusion on a few images of a subject (e.g., a face).
- Use LoRA for parameter‑efficient fine‑tuning.

## Topics Covered
1. Preparing a small dataset (4–5 images of a subject).
2. Writing a DreamBooth training script with Diffusers + PEFT (LoRA).
3. Generating new images of the subject in different contexts.

## Setup
```bash
pip install diffusers accelerate peft transformers datasets torch xformers