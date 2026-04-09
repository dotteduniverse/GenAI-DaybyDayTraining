# Day 1 – Optional Exercises

Complete at least **two** of the following exercises to reinforce your understanding.

### Exercise 1: Prompt diversity with GPT‑2
Generate text for **five different starting prompts** (e.g., *“Once upon a time”*, *“The secret to happiness is”*, *“If I could travel anywhere”*).  
For each prompt, use two different temperatures (0.2 and 1.0).  
Write a short observation: how does the output change with temperature and prompt style?

### Exercise 2: Compare image generation models
Instead of Stable Diffusion v1.5, try another model from Hugging Face, e.g.:
- `"dreamlike-art/dreamlike-photoreal-2.0"` (photorealistic)
- `"prompthero/openjourney"` (artistic)

Generate the same prompt (e.g., *“a robot reading a book in a library”*) with both models.  
Compare the results: which one do you prefer and why?

### Exercise 3: Use the Hugging Face Inference API (no local download)
If you have a Hugging Face token (free), use the `requests` library to call the inference API for text generation:

```python
import requests

API_URL = "https://api-inference.huggingface.co/models/gpt2"
headers = {"Authorization": "Bearer YOUR_HF_TOKEN"}
payload = {"inputs": "The meaning of life is", "parameters": {"max_length": 50}}

response = requests.post(API_URL, headers=headers, json=payload)
print(response.json())