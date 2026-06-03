# Exercises – Day 43

1. **Build a Gradio interface for your project**  
   Implement the core function (e.g., LLM call, image generation). Include at least two input controls (text, slider, image, etc.).

2. **Add a loading indicator**  
   In Gradio, use `gr.Progress()` or a simple `queue` to show processing. In Streamlit, use `st.spinner()`.

3. **Deploy temporarily**  
   Run `share=True` in Gradio to create a public 72‑hour link. Share the link with a peer.

4. **Error handling**  
   If the model fails, display a friendly error message instead of a crash. Test by simulating an error (e.g., remove API key temporarily).

5. **Bonus: Streamlit chat interface**  
   Use `st.chat_message` and session state to create a chatbot with conversation history.