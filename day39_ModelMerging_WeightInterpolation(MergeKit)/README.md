# Day 39: Model Merging & Weight Interpolation (MergeKit)

## Learning Goals
- Understand the concept of model merging: combining multiple fine-tuned models into one without additional training.
- Learn how to use MergeKit to perform different merging strategies: Linear, SLERP, TIES, and DARE‑TIES.
- Merge two or more language models and deploy the result.

## Topics Covered
1. Installation of MergeKit.
2. YAML configuration for merging models.
3. Linear (weighted average) and SLERP (spherical linear interpolation) methods.
4. Advanced methods: TIES, DARE‑TIES for reducing interference.
5. Running the merge and testing the merged model.

## Setup
```bash
# From GitHub (recommended)
git clone https://github.com/arcee-ai/mergekit.git
cd mergekit
pip install -e .

# Or via PyPI
pip install mergekit