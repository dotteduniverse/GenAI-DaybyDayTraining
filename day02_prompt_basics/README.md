
---

## Day 2 – Prompt Engineering Basics

### `day02_prompt_basics/README.md`

```markdown
# Day 2 – Prompt Engineering Basics

## 🎯 Learning Objectives
- Understand what a prompt is and how it guides an LLM.
- Learn core prompt components: instruction, context, input data, output indicator.
- Write 10 diverse prompts and compare the model’s responses.
- Discover how small wording changes affect output quality.
- Learn about zero‑shot, few‑shot, and role‑based prompting.

## 📚 Detailed Concepts

### What is a prompt?
A prompt is the input you give to a language model to elicit a desired output.  
It can be as simple as a question (“What is the capital of France?”) or as complex as a multi‑paragraph instruction with examples.

### Core components of a good prompt
1. **Instruction** – what you want the model to do (e.g., “Translate”, “Summarise”, “Explain”).
2. **Context** – background information (e.g., “You are a travel agent…”).
3. **Input data** – the specific thing to process (e.g., the text to translate).
4. **Output indicator** – how you want the answer formatted (e.g., “Answer in one sentence:” or “Output JSON:”).

### Prompting techniques
- **Zero‑shot**: No examples given. E.g., *“Classify this review as positive or negative: 'I love this!'”*
- **Few‑shot**: Provide 2–3 examples before asking. Great for teaching new tasks.
- **Role prompting**: “You are a professional chef. Write a recipe for…” – changes style and content.
- **Chain‑of‑thought**: Ask the model to reason step by step, often improving accuracy on math/logic.
- **Negative instructions**: “Do NOT use technical jargon” – can reduce unwanted behaviours.

### Why prompt engineering matters
- A well‑crafted prompt can **double accuracy** and reduce hallucinations.
- Saves money (fewer tokens) and latency.
- Allows you to control style, tone, and format without fine‑tuning.

## 🛠️ Setup
You need an OpenAI API key (or alternative like Cohere / local LLM).  
If you haven’t already, add your key to the `.env` file in the repo root:
