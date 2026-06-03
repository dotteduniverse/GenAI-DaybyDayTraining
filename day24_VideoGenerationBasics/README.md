# Day 24: Video Generation Basics (Stable Video Diffusion)

## Learning Goals
- Understand how Stable Video Diffusion (SVD) generates short video clips from a single image.
- Learn to control motion, frame rate, and looping.
- Generate a short looping animation.

## Topics Covered
1. Loading Stable Video Diffusion from Hugging Face Diffusers.
2. Generating a video from a static image.
3. Creating a looping animation by reversing or blending frames.
4. Saving output as an MP4 or GIF.

## Setup
```bash
pip install diffusers transformers accelerate safetensors imageio imageio-ffmpeg pillow matplotlib