# Exercises – Day 37

1. **Try different prompts**  
   Generate 3D models for “a chair”, “a sports car”, “a tree”. Compare the mesh quality.

2. **Adjust guidance scale**  
   Vary guidance_scale (5.0, 10.0, 20.0). How does it affect adherence to the prompt?

3. **Generate multiple views**  
   Instead of a mesh, generate 6‑view images of the object using `decode_latent_images()`. Display them in a grid.

4. **Export to different formats**  
   Save as `.glb` (for web) using `trimesh` or `open3d`. Load the `.glb` in a browser.

5. **Bonus: NeRF conceptual**  
   Write a short explanation (2 paragraphs) of how NeRFs differ from Shap‑E’s approach.