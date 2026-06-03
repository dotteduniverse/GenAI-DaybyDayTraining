# Exercises – Day 25 (Mini Project)

1. **Expand the dataset**  
   Add at least 20 more images of your own (or download from Unsplash). Rebuild the index. Test a few text queries (e.g., “mountain”, “food”, “city”).

2. **Image‑to‑image search accuracy**  
   Pick one image as query. Does the search return visually similar images? Try with a very different image (e.g., a car vs a cat). Report the top 3 results.

3. **Precision at k**  
   For a given text query (“dog”), manually label which images in your collection are relevant. Compute precision@3 and precision@5.

4. **Save and load the index**  
   Use `faiss.write_index()` and `faiss.read_index()` so you don’t recompute embeddings every time. Also save the list of image paths.

5. **Bonus: Web interface**  
   Use Gradio to create a simple UI: an input box for text or an image uploader, then display the retrieved images with similarity scores.