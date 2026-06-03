# Exercises – Day 35

1. **Add a summariser tool**  
   Create a tool that takes a URL and returns a short summary (using LLM). Integrate it into the agent.

2. **Cite sources**  
   Modify the final output to include numbered references and inline citations (e.g., `[1]`). Ensure each claim has a source.

3. **Limit token usage**  
   Implement a token budget: if a scraped page exceeds 4000 chars, summarise it before feeding to the final synthesis.

4. **Save report to file**  
   Write the final research report to a Markdown file with headings and a table of contents.

5. **Bonus: Multi‑query refinement**  
   After the first search, ask the agent to identify gaps and perform a second search for missing information.