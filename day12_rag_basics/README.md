# Day 12 – Retrieval‑Augmented Generation (RAG) Basics

## 🎯 Learning Objectives
- Understand the RAG architecture (retriever + generator).
- Build a simple RAG pipeline using LangChain + ChromaDB.
- Answer questions based on a custom document collection.

## 📚 Detailed Concepts

### Why RAG?
LLMs have limited context and can hallucinate. RAG provides **up‑to‑date, factual information** by retrieving relevant documents from a knowledge base and feeding them to the LLM.

### RAG pipeline
1. **Ingest** – Split documents into chunks, embed them, store in a vector database.
2. **Retrieve** – For a query, embed it, find top‑k similar chunks (cosine similarity).
3. **Generate** – Inject retrieved chunks into the prompt and ask the LLM to answer.

### Components
- **Embedding model** – e.g., `all-MiniLM-L6-v2` or OpenAI `text-embedding-ada-002`.
- **Vector database** – ChromaDB (lightweight), FAISS, Pinecone, Weaviate.
- **LLM** – any chat model (OpenAI, local).

### LangChain
A framework for building applications with LLMs. It provides:
- Document loaders (PDF, text, web).
- Text splitters (recursive character, semantic).
- Vector stores (Chroma, FAISS).
- Chains (RetrievalQA).

## 🛠️ Setup
```bash
pip install langchain chromadb openai tiktoken