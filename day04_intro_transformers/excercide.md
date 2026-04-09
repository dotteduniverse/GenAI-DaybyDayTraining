# Day 4 – Exercises

1. **Model size vs. speed** – Load `gpt2`, `gpt2-medium`, `gpt2-large`. Generate a 100‑token output and measure time using `time.time()`. Which is fastest? Which produces the most coherent output?
2. **Batch generation** – Generate 3 different completions for the same prompt using `num_return_sequences=3`. Compare diversity.
3. **Manual tokenisation** – Tokenise a sentence, print token IDs, then decode back. Add special tokens manually.
4. **Advanced** – Use `model.generate()` with parameters `top_k=50`, `top_p=0.9`, `repetition_penalty=1.2`. Explain what each does.