# Exercises – Day 29

1. **Compare LLM judge vs OpenAI Moderation API**  
   Run 10 test inputs (some safe, some unsafe) through both. Calculate precision and recall for the LLM judge (treat OpenAI API as ground truth).

2. **Add a confidence score**  
   Modify the judge to output a confidence percentage (0–100) along with the verdict.

3. **Threshold tuning**  
   Implement a reject threshold: if confidence < 70%, ask a human moderator or block the request.

4. **Evaluate on edge cases**  
   Test the judge on ambiguous inputs (e.g., sarcasm, jokes with mild profanity). Does it over‑censor?

5. **Bonus: Guardrails for agent tools**  
   Integrate the judge into the tool‑using agent from day 26: before executing a tool, moderate the tool input and output.