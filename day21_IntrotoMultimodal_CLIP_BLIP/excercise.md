# Exercises – Day 21

1. **Different images**  
   Test CLIP zero‑shot on three images of your choice (e.g., a dog, a landscape, a screenshot). Use at least 5 candidate labels per image. Report the top‑1 label and its probability.

2. **Custom label sets**  
   For the cat image, use these labels: `["a kitten", "an adult cat", "a tiger", "a lion"]`.  
   Does CLIP correctly choose “a kitten”? Explain why or why not.

3. **BLIP on challenging images**  
   Run BLIP on an image containing multiple objects (e.g., a street scene) and on an abstract painting. Compare the quality of captions.

4. **Cosine similarity between image and text**  
   Instead of classification, manually compute the cosine similarity between CLIP’s image embedding and each text embedding. Normalise the vectors first. Use `torch.nn.functional.cosine_similarity`.

5. **Bonus: Multimodal retrieval**  
   Download 5–10 images into a folder. Given a text query (e.g., “a blue car”), use CLIP to find the image most similar to the text. Print the filename and similarity score.