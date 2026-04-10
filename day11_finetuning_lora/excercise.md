# Day 11 – Exercises

1. **Different domain** – Fine‑tune on a dataset of your choice (e.g., movie scripts, technical support Q&A). Use at least 100 examples.
2. **Vary rank (r)** – Train with r=2, r=8, r=32. Compare the number of trainable parameters and output quality.
3. **Merge and save** – Use `model.merge_and_unload()` to merge LoRA weights into the base model and save the full model.
4. **Load adapter only** – Save the adapter, then load it onto a fresh base model using `PeftModel.from_pretrained()`.