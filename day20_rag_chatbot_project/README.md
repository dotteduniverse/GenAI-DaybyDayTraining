# Day 20 – Mini Project: RAG Chatbot for a PDF Collection

## 🎯 Learning Objectives
- Build a complete RAG chatbot over a collection of PDF documents.
- Add conversation memory.
- Deploy as a simple Gradio or Streamlit app.

## 📚 Detailed Concepts

### Project scope
You will build a chatbot that:
- Ingests a folder of PDFs (e.g., research papers, product manuals).
- Splits and indexes them.
- Answers questions about the content, remembering conversation context.

### Components
1. **Document ingestion** – `PyPDFLoader`, `RecursiveCharacterTextSplitter`.
2. **Vector store** – ChromaDB or FAISS.
3. **Retrieval** – top‑k similarity search.
4. **LLM** – OpenAI or local.
5. **Memory** – `ConversationBufferMemory`.
6. **UI** – Gradio or Streamlit.

### Optimisation tips
- Use `ConversationalRetrievalChain` from LangChain.
- Handle long conversations by summarising old history.
- Add source citation: show which PDF page the answer came from.

## 🛠️ Setup
```bash
pip install langchain chromadb openai pypdf gradio