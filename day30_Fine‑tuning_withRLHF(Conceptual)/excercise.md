# Exercises – Day 30

1. **Prepare a custom preference dataset**  
   Create a small JSON file with 10 examples, each containing `"chosen"` and `"rejected"` responses to a prompt. Load it using `datasets.load_dataset("json", data_files="my_data.json")`.

2. **Train on a smaller model**  
   Use `"distilgpt2"` instead of `"gpt2"` to reduce memory. Train for 1 epoch and observe loss decrease.

3. **Evaluate reward model**  
   After training (even a few steps), compute the accuracy on a validation set: the reward for `chosen` should be higher than for `rejected` on most examples.

4. **Conceptual: PPO loop**  
   Write pseudocode for the PPO training loop using the trained reward model to fine‑tune a policy model.

5. **Bonus: Use LoRA**  
   Modify the training to use `peft` (LoRA) to make reward model training more efficient.