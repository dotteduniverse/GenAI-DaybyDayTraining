# Day 15 – Structured Output: JSON Mode & Function Calling

## 🎯 Learning Objectives
- Force LLMs to output valid JSON for easy parsing.
- Use OpenAI's function calling to get structured data.
- Extract information from messy text into a schema.

## 📚 Detailed Concepts

### Why structured output?
LLMs naturally output free text, but applications often need JSON, XML, or specific fields.  
Structured output enables:
- Automatic data extraction (e.g., from emails).
- Integration with APIs.
- Reliable downstream processing.

### Methods
1. **Prompt engineering** – *“Output JSON with keys: name, age.”* Works but may sometimes produce invalid JSON.
2. **JSON mode** (OpenAI) – Set `response_format={"type": "json_object"}`. Guarantees valid JSON.
3. **Function calling** – Define a function schema, the model returns a structured argument object.

### OpenAI function calling
Define functions with parameters (JSON Schema). The model decides whether to call a function and returns the arguments.  
You don't need to execute the function – you can just use the arguments as structured output.

### Other providers
- Cohere: `json_mode` parameter.
- Anthropic: `{ "type": "json_object" }` in system prompt + explicit instruction.
- Local models: use `guidance` or `outlines` library.

## 🛠️ Setup
```bash
pip install openai