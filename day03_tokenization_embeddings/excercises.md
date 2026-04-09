# Day 3 – Optional Exercises

Complete at least **two** of the following.

### Exercise 1: Token cost estimator
Write a function that takes a text file path, reads it, and estimates the cost to process it with GPT-3.5-turbo (assume $0.0015 per 1k tokens).  
Test it on a chapter of a public domain book (e.g., from Project Gutenberg).

### Exercise 2: Find the odd one out
Use the sentence embeddings and cosine similarity to find which sentence in a list is least similar to the others.  
Example list:  
`["I love pizza.", "Pasta is delicious.", "The weather is nice today.", "Spaghetti with meatballs is great."]`

### Exercise 3: Visualise embeddings with PCA
Take the 4 sentence embeddings from the notebook. Use `sklearn.decomposition.PCA` to reduce them to 2 dimensions, then plot them as a scatter plot with labels.  
Observe which sentences cluster together.

### Exercise 4: Multilingual tokenisation comparison
Take the same sentence in 3 different languages (e.g., English, Spanish, Japanese).  
Tokenise each with `cl100k_base` and compare the number of tokens.  
Which language is most token‑efficient? Which is least?

### Exercise 5: Embedding search engine
Create a small search engine:
- Embed 20 sentences (e.g., from a Wikipedia article).
- Ask the user for a query, embed the query, and return the top‑3 most similar sentences from the collection.

---

💡 **Share your odd‑one‑out result** – post the sentence that was least similar and explain why.