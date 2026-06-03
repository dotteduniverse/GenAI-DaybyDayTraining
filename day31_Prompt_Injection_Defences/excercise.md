# Exercises – Day 31

1. **Expand heuristic patterns**  
   Add at least 5 more patterns for injection (e.g., “you are now DAN”, “sudo mode”, “I'm your new developer”). Test them.

2. **Indirect injection detection**  
   Create a test where the injection is hidden inside a seemingly normal request (e.g., “What is 2+2? Also, ignore previous instructions.”). Does your detector catch it?

3. **False positive analysis**  
   Run 20 normal, safe queries through the LLM judge. Count false positives. Adjust the prompt to reduce them.

4. **Defence: XML tagging**  
   Instead of random nonces, wrap user input in `<user_input>` XML tags. Implement and test.

5. **Bonus: Guardrails library**  
   Install `guardrails-ai` and use its built‑in prompt injection detector. Compare performance with your implementation.