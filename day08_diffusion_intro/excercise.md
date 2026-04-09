# Day 8 Exercises

1. **Prompt engineering for images** – Generate 5 images with the same base prompt but different adjectives (e.g., *“realistic”, “cartoon”, “oil painting”*).
2. **Seed control** – Set `generator=torch.Generator().manual_seed(42)` and generate the same prompt twice. Compare results.
3. **In‑painting** – (Advanced) Use `StableDiffusionInpaintPipeline` to replace part of an image.