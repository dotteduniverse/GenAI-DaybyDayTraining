# Day 25: Mini Project – Multimodal Search Engine (CLIP + FAISS)

## Learning Goals
- Combine CLIP embeddings for both images and text in a single vector space.
- Build a FAISS index over a collection of images.
- Support both text‑to‑image and image‑to‑image search.

## Project Overview
You will create a search engine that takes either a **text query** or an **image query** and returns the most relevant images from a local dataset.

## Topics Covered
1. Generating CLIP embeddings for images and text.
2. Building a FAISS index with image embeddings.
3. Querying with text or another image.
4. Displaying results with similarity scores.

## Setup
```bash
pip install faiss-cpu pillow torch transformers matplotlib scikit-learn