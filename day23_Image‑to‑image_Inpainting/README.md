# Day 23: Image‑to‑Image & Inpainting

## Learning Goals
- Understand how to use Stable Diffusion for image‑to‑image generation (starting from an initial image).
- Perform inpainting: selectively regenerate parts of an image using a mask.
- Learn the role of `denoising_strength` in img2img.

## Topics Covered
1. Loading a Stable Diffusion img2img pipeline.
2. Transforming an existing image with a text prompt.
3. Loading an inpainting pipeline and using a mask to edit specific regions.

## Setup
```bash
pip install diffusers transformers accelerate safetensors pillow matplotlib