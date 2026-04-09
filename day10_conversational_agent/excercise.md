# Day 10 Exercises

1. **Token limit** – Write a function that counts tokens (using `tiktoken`) and when the total exceeds 3000, removes the oldest non‑system message.
2. **Persona switch** – Let the user change the system message with `!persona pirate` or similar.
3. **Save chat** – Implement `!save filename.txt` that writes the conversation to a file.
4. **Streaming** – Modify the loop to stream tokens using `stream=True` and print them incrementally.