# Exercises – Day 42

1. **Collect your own data**  
   For your capstone project, collect at least 50 raw examples (text, images, or audio). Document the source.

2. **Clean and preprocess**  
   Write a cleaning function specific to your data type. Remove duplicates and irrelevant content.

3. **Create chunks or segments**  
   If your project involves RAG or long documents, split into chunks. If it’s image generation, create a metadata CSV with image paths and captions.

4. **Split into train/val/test**  
   Use `sklearn.model_selection.train_test_split` to create 80/10/10 splits. Save each split separately.

5. **Bonus: Data augmentation**  
   For images, apply random rotations, flips, or color jitter. For text, use back‑translation or synonym replacement.