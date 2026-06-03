# Day 37: Text‑to‑3D & NeRF Basics

## Learning Goals
- Understand the basics of text‑to‑3D generation.
- Use OpenAI’s Shap‑E to generate 3D meshes from text prompts.
- Visualise and export the generated 3D object.

## Topics Covered
1. Installing and loading Shap‑E model.
2. Generating a 3D point cloud or mesh from a text prompt.
3. Visualising the 3D object in a notebook or saving as `.obj`/`.glb`.

## Setup
```bash
pip install torch shap-e trimesh matplotlib open3d