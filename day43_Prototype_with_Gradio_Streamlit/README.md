# Day 43: Prototype with Gradio / Streamlit

## Learning Goals
- Build an interactive web UI for your GenAI model using Gradio or Streamlit.
- Understand the trade‑offs between the two frameworks.
- Deploy the prototype locally and optionally to a public URL.

## Topics Covered
1. Gradio: simple UI with `gr.Interface`, custom components, and live demos.
2. Streamlit: script‑based UI with state management and caching.
3. Connecting your model (e.g., LLM, image generator, RAG chain) to the UI.
4. Adding file uploads, sliders, text inputs, and output displays.

## Setup
```bash
pip install gradio streamlit