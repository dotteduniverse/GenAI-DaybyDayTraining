# Exercises – Day 26

1. **Add a new tool**  
   Create a tool that fetches the current weather for a given city (use OpenWeatherMap API). Integrate it into the agent.

2. **Change the LLM**  
   Replace `gpt-4o` with a local model via Ollama (e.g., `llama3`). Modify the code accordingly.

3. **Parallel tool calls**  
   LangGraph already handles parallel tool calls. Ask the agent a question that requires both calculator and search. Observe the order.

4. **Limit tool usage**  
   Add a maximum number of tool‑calling steps (e.g., 3) to prevent infinite loops.

5. **Bonus: AutoGen alternative**  
   Install `pyautogen` and build a similar tool‑using agent using AutoGen’s `AssistantAgent` and `UserProxyAgent`.