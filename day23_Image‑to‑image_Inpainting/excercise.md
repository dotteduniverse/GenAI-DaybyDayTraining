# Exercises – Day 23

1. **Style transfer with img2img**  
   Take a photo of a building. Use img2img with prompt “a watercolor painting of a building” and try different strengths (0.3, 0.6, 0.9). Show the results.

2. **Inpaint an object away**  
   Use an image with a person or an object. Create a mask covering the object. Use prompt “background, empty space” (or no prompt) to remove it. Does it work convincingly?

3. **Add a new object**  
   In a landscape image, mask a region where you want to add, e.g., “a red balloon”. Use inpainting to insert it. Experiment with different mask shapes.

4. **Strength vs. steps**  
   Keep strength fixed at 0.5, vary inference steps (10, 25, 50). How does the output change? Is higher steps always better?

5. **Bonus: Inpaint with custom mask from segmentation**  
   Use a segmentation model (e.g., `detectron2` or a simple color threshold) to automatically generate a mask for a specific object (e.g., the sky). Then replace the sky with “a starry night”.