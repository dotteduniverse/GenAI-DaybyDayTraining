# Exercises – Day 34

1. **Use your own long document**  
   Replace the sample text with a PDF or a long article (e.g., Wikipedia page of a topic). Implement PDF loading with `PyPDFLoader` from LangChain.

2. **Chunk size experiment**  
   Try chunk sizes of 1000, 2000, and 4000 characters. Measure the quality of the final summary and the number of API calls.

3. **Custom reduce prompt**  
   Modify the reduce prompt to output a bullet‑point summary instead of prose.

4. **Refine chain alternative**  
   Use `chain_type="refine"` instead of `"map_reduce"`. Compare the output and API cost.

5. **Bonus: Streaming map‑reduce**  
   Implement a manual map‑reduce loop that streams each chunk’s summary as it finishes, then combines at the end.