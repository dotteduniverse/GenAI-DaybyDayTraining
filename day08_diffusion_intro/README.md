# Day 8 – Introduction to Image Generation with Diffusion Models

## 🎯 Learning Objectives
- Understand the diffusion process (forward noise, reverse denoising).
- Generate an image using Stable Diffusion via Hugging Face `diffusers`.
- Experiment with prompts and guidance scale.

## 📚 Concepts Covered
- How diffusion models work (high‑level).
- The role of the UNet and text encoder (CLIP).
- Guidance scale: how closely to follow the prompt.

## 🛠️ Setup
```bash
pip install diffusers transformers accelerate torch