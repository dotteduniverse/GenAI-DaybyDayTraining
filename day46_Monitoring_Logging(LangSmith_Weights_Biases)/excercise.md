# Exercises – Day 46

1. **Set up LangSmith**  
   Create an account at [smith.langchain.com](https://smith.langchain.com), get an API key. Set environment variables and run the notebook. Verify traces appear in the UI.

2. **Add custom feedback**  
   Use `client.create_feedback()` to add a user rating (1-5) to a specific run ID. Retrieve the run ID from the trace URL.

3. **Log to WandB**  
   Modify your capstone code to log at least 10 interactions (prompt, response, latency, token count). View the logged data in WandB tables.

4. **Monitor a deployed Space**  
   If you deployed to HF Spaces in Day 45, add LangSmith tracing to the app (install langsmith, set env vars as secrets). Trigger a few calls and confirm traces appear.

5. **Bonus: Cost tracking**  
   Use `tiktoken` to count tokens and log the cost per call (`cost = tokens * 0.000002` for GPT-3.5‑turbo). Display a running total in WandB.