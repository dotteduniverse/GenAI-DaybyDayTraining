# Day 1 – What is Generative AI? Exploring Famous Models

## 🎯 Learning Objectives
- Define Generative AI and distinguish it from discriminative AI.
- Understand real‑world applications (text, image, code, music, video).
- Get hands‑on with two landmark models:
  - **GPT‑2** (text generation)
  - **Stable Diffusion** (image generation)
- Experience how prompts and parameters affect output.

## 📚 Detailed Concepts

### Generative vs. Discriminative AI
- **Discriminative models** learn boundaries between classes (e.g., “is this a cat or a dog?”).  
- **Generative models** learn the underlying distribution of the data and can **create new samples** (e.g., write a new sentence, draw a new image).

### How GPT‑2 works (simplified)
- GPT‑2 is a **causal language model** – it predicts the next word given previous words.
- It uses a **transformer decoder** architecture with multi‑head self‑attention.
- The model was trained on 8 million web pages (40 GB text) and has 124 million parameters (small version).
- During generation, it samples from the probability distribution over the next token.

### How Stable Diffusion works (intuitive)
- **Diffusion process**: take an image → add noise step by step until it becomes pure noise.  
- **Reverse process**: learn to remove noise step by step, guided by a text prompt.
- **Components**:  
  - **Text encoder** (CLIP) turns prompt into embeddings.  
  - **UNet** predicts the noise to remove.  
  - **VAE** compresses image to latent space for efficiency.

### Real‑world applications
- **Text**: ChatGPT, GitHub Copilot, Jasper.
- **Image**: Midjourney, DALL‑E, Adobe Firefly.
- **Code**: CodeWhisperer, Codeium.
- **Music**: MusicLM, Jukebox.
- **Video**: Runway Gen‑2, Pika Labs.

## 🛠️ Setup (first time only)
```bash
pip install transformers torch diffusers accelerate