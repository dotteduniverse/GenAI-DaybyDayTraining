# Day 42: Data Collection & Preprocessing

## Learning Goals
- Understand how to gather and prepare a dataset for your GenAI project.
- Learn common preprocessing techniques: cleaning, formatting, splitting, augmentation.
- Create a reusable data pipeline.

## Topics Covered
1. Sources of data: web scraping, APIs, public datasets, user uploads.
2. Cleaning: removing duplicates, handling missing values, standardising formats.
3. Preprocessing for different modalities: text (chunking, tokenisation), images (resizing, normalisation), audio (resampling).
4. Splitting into train/validation/test sets.
5. Storing the dataset (JSON, CSV, Hugging Face Datasets, or vector DB).

## Setup
```bash
pip install datasets pandas requests beautifulsoup4 Pillow