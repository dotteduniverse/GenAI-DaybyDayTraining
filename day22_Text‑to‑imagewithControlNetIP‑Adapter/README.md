# Day 22: Text‑to‑Image with Control (ControlNet, IP‑Adapter)

## Learning Goals
- Understand how ControlNet adds spatial control (edges, pose, sketch) to Stable Diffusion.
- Use a sketch image as input to guide the generation.
- Optionally explore IP‑Adapter for image‑prompt conditioning.

## Topics Covered
1. Loading Stable Diffusion + ControlNet (sketch or canny) from Diffusers.
2. Generating an image conditioned on a sketch + text prompt.
3. (Bonus) Using IP‑Adapter for subject‑driven generation.

## Setup
```bash
pip install diffusers transformers accelerate safetensors opencv-python pillow matplotlib