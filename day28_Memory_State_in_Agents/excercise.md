# Exercises – Day 28

1. **Persist long‑term memory**  
   Save the long‑term memory facts to a JSON file and load them on restart. Modify the agent to use this.

2. **Automatic fact extraction**  
   Instead of relying on keywords, ask an LLM to extract any personal facts from each user message and add them to long‑term memory.

3. **Forgetting mechanism**  
   Implement a decay or removal policy: if a fact hasn't been retrieved in the last N interactions, delete it.

4. **Hybrid memory retrieval**  
   Combine recent short‑term messages and long‑term facts into a single rank‑based list (e.g., recency score + relevance score).

5. **Bonus: Memory‑aware agent with LangGraph**  
   Integrate the memory classes into the LangGraph agent from day 26.