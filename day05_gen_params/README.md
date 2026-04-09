
---

## Day 5 – Text Generation Parameters (Temperature, Top‑p, etc.)

### `day05_gen_params/README.md`

```markdown
# Day 5 – Text Generation Parameters

## 🎯 Learning Objectives
- Understand how generation parameters control output.
- Experiment with temperature, top‑k, top‑p, repetition penalty.
- Build an interactive text generator with sliders (Gradio).

## 📚 Detailed Concepts

### How text generation works at each step
1. The model outputs a vector of **logits** (raw scores) for every possible token in the vocabulary.
2. These logits are converted to probabilities using **softmax**.
3. The next token is chosen based on the sampling strategy.

### Key parameters

#### Temperature
- Formula: `logits = logits / temperature` before softmax.
- Low temperature (e.g., 0.2): sharp distribution → high‑probability tokens become much more likely. Output is deterministic, repetitive.
- High temperature (e.g., 1.5): flatter distribution → more equal chance for many tokens. Output is more random, creative, sometimes nonsensical.
- `temperature = 0` is not allowed (division by zero). Use `do_sample=False` for greedy.

#### Top‑k sampling
- Keep only the **k** tokens with the highest probabilities, renormalise.
- Example: `top_k=50` – only the top 50 tokens can be chosen.
- Removes very low‑probability tokens (which are often nonsense).

#### Top‑p (nucleus sampling)
- Keep the smallest set of tokens whose cumulative probability ≥ p.
- Example: `top_p=0.9` – include tokens until their probabilities sum to 0.9.
- Adaptive – includes more tokens when distribution is flat, fewer when it’s sharp.
- Often used together with top‑k (e.g., `top_k=50, top_p=0.95`).

#### Repetition penalty
- Penalises tokens that have already appeared in the generated text.
- `repetition_penalty=1.0` (default) – no penalty.
- `1.2` – mild penalty; `1.5` – strong penalty.
- Too high can cause incoherence.

### Practical guidelines
- **Factual answers** (Q&A, translation): low temperature (0.0–0.3), no sampling (greedy) or very low top‑p.
- **Creative writing**: temperature 0.7–1.0, top‑p 0.9, repetition penalty 1.1–1.2.
- **Code generation**: temperature 0.2–0.4, top‑p 0.95.
- **Story generation with character consistency**: lower temperature, higher repetition penalty.

## 🛠️ Setup
```bash
pip install transformers gradio