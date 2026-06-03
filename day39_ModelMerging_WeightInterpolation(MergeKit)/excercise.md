# Exercises – Day 39

1. **Linear merge of two models**  
   Merge `microsoft/phi-2` with `cognitivecomputations/dolphin-2_6-phi-2` using a linear merge with weights 0.4/0.6. Run the merge (use `--cuda` if available). Load and test the merged model with a prompt like "What is the capital of France?".

2. **Compare merging methods**  
   Perform three merges on the same two models using: Linear (equal weights), SLERP (t=0.5), and TIES. Generate the same prompt for each merged model. Compare the quality, coherence, and style of the outputs.

3. **Three‑model merge**  
   Add a third model to your configuration (e.g., `HuggingFaceH4/zephyr-7b-beta`). Merge all three with equal weights. Does the quality improve?

4. **Density parameter in TIES**  
   TIES has a `density` parameter (usually 0.5). Try densities of 0.3, 0.5, and 0.8. Observe how it affects the merged model's behaviour. (Hint: lower density = more sparsity, potentially less interference but also less retained knowledge.)

5. **Bonus: DARE‑TIES**  
   DARE (Drop And REscale) is an extension that randomly drops parameters before merging to reduce interference. Try `merge_method: dare_ties` in your config. Compare with standard TIES.