# Day 8 – Introduction to Image Generation with Diffusion Models

## 🎯 Learning Objectives
- Understand the diffusion process (forward noise, reverse denoising).
- Generate an image using Stable Diffusion via Hugging Face `diffusers`.
- Experiment with prompts and guidance scale.

## 📚 Detailed Concepts

### How diffusion models work (intuitive)
1. **Forward process**: take a real image, add a little Gaussian noise repeatedly until it becomes pure random noise (like static on a TV).
2. **Reverse process**: train a neural network (UNet) to predict the noise that was added at each step. Starting from pure noise, the model gradually removes noise to recreate the original image.
3. **Conditioning**: to generate images from text, we add a **text encoder** (CLIP) that turns the prompt into embeddings. The UNet learns to remove noise in a way that matches the prompt.

### Key components of Stable Diffusion
- **VAE (Variational Autoencoder)**: compresses the image from pixel space (512x512x3) to a smaller latent space (64x64x4). This makes diffusion much faster.
- **Text encoder (CLIP)**: converts text prompt into a 77‑token embedding.
- **UNet**: the noise predictor. Operates in the latent space.
- **Scheduler**: controls how noise is added and removed (e.g., DDPM, LMS, PNDM).

### Guidance scale (classifier‑free guidance)
- Controls how strongly the model follows the prompt.
- Formula: `denoised = denoised_unconditional + guidance_scale * (denoised_conditional - denoised_unconditional)`
- Low (1‑3): more creative, may ignore parts of prompt.
- Medium (7‑9): good balance.
- High (15‑20): very faithful to prompt, but may look unnatural.

### Negative prompt
What you *don’t* want to see.  
Example: `negative_prompt="blurry, ugly, distorted, bad anatomy"`  
The model tries to move away from those concepts.

## 🛠️ Setup
```bash
pip install diffusers transformers accelerate torch