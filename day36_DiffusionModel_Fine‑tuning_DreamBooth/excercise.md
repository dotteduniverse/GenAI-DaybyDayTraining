# Exercises – Day 36

1. **Collect your own dataset**  
   Take 5–10 photos of an object or person (ensure variety, square crop to 512x512). Run DreamBooth training.

2. **Change the identifier**  
   Replace `sks person` with a more meaningful identifier like `mycat` or `mytoy`. Does it affect generation quality?

3. **Training steps experiment**  
   Train for 200, 500, and 800 steps. Generate the same prompt and compare overfitting vs. quality.

4. **Class‑specific prior preservation**  
   Enable prior preservation loss by adding `--with_prior_preservation --class_data_dir=./class_data --class_prompt="a person"`. Observe changes.

5. **Bonus: Merge LoRA with another style LoRA**  
   Use `pipe.load_lora_weights()` to load two LoRAs (e.g., DreamBooth face + anime style). Generate a hybrid result.