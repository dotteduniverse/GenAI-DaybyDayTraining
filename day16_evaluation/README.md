# Day 16 – Evaluating LLMs: BLEU, ROUGE, Custom Metrics

## 🎯 Learning Objectives
- Understand common automatic evaluation metrics for text generation.
- Compute BLEU (machine translation) and ROUGE (summarisation).
- Build a custom evaluator using an LLM as a judge.

## 📚 Detailed Concepts

### Why evaluate?
To compare models, prompts, or fine‑tunes. Metrics provide a quantitative measure of quality.

### BLEU (Bilingual Evaluation Understudy)
- Measures n‑gram overlap between generated and reference text.
- Ranges 0–1 (1 = identical). Used for translation.
- Weaknesses: ignores meaning, favours short outputs.

### ROUGE (Recall‑Oriented Understudy for Gisting Evaluation)
- Measures recall of n‑grams (ROUGE‑N) or longest common subsequence (ROUGE‑L).
- Common for summarisation.

### BERTScore
- Uses BERT embeddings to compute similarity, capturing meaning better than n‑grams.

### LLM as a judge
- Use a strong LLM (e.g., GPT‑4) to rate outputs on a scale (1‑5) or compare two outputs.
- Can be more aligned with human preferences.

## 🛠️ Setup
```bash
pip install evaluate nltk rouge-score bert-score