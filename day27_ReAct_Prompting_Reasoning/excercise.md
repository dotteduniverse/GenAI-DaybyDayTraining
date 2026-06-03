# Exercises – Day 27

1. **Add a new tool**  
   Implement a `Weather[city]` tool using an API. Integrate it into the ReAct prompt and parser.

2. **Handle errors gracefully**  
   Modify the agent to retry up to 2 times if a tool returns an error (e.g., “Not found”).

3. **Limit thought length**  
   Add a maximum token limit per thought to prevent overly long reasoning.

4. **Compare with LangGraph**  
   Rewrite the same agent using LangGraph (from day 26). Which is easier to extend?

5. **Bonus: Multi‑turn conversations**  
   Extend the agent to maintain a conversation memory across multiple user questions.