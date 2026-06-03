# Day 34: Working with Very Long Context (100k+)

## Learning Goals
- Understand challenges of processing documents that exceed LLM context windows.
- Implement a map‑reduce summarisation strategy: split, summarise chunks, then combine.
- Use LangChain’s `load_summarize_chain` with `MapReduceDocumentsChain`.

## Topics Covered
1. Loading a long document (e.g., a book or long PDF).
2. Splitting into chunks with overlap.
3. Mapping: summarise each chunk independently.
4. Reducing: combine chunk summaries into a final summary.

## Setup
```bash
pip install langchain langchain-openai tiktoken