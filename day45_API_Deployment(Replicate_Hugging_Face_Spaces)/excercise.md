# Exercises – Day 45

1. **Create a Hugging Face Space**  
   Use the folder generated above (or your own) to create a new Space. Set `sdk: gradio` or `streamlit`. Add your API keys as secrets (HF Settings → Secrets).

2. **Test the live Space**  
   After deployment, share the public URL. Send at least 5 test inputs to confirm it works.

3. **Deploy a custom model**  
   Instead of calling OpenAI, use a free open‑source model (e.g., `microsoft/phi-2`) loaded via Transformers. Note: It may be slow on free CPU tier.

4. **Add environment variables**  
   For OpenAI API key, set it as a secret in HF Spaces. Modify your `app.py` to read `os.getenv("OPENAI_API_KEY")`.

5. **Bonus: Deploy to Replicate**  
   Create a Replicate model (requires a paid or trial account). Use `cog init` to scaffold, then `cog push`. Share the public API endpoint.