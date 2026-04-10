# Day 18 – Quantisation: GGUF, GPTQ

## 🎯 Learning Objectives
- Understand quantisation: reducing model precision (FP16 → INT4).
- Load a 4‑bit quantised model on a laptop.
- Compare quality vs. size trade‑offs.

## 📚 Detailed Concepts

### What is quantisation?
Neural networks are trained in FP32 or FP16. Quantisation converts weights to lower precision (e.g., INT8, INT4).  
- **FP16**: 2 bytes per parameter.  
- **INT8**: 1 byte (4x smaller).  
- **INT4**: 0.5 bytes (8x smaller).  

### Methods
- **GPTQ** (GPT Quantisation) – optimised for GPU, 4‑bit, minimal accuracy loss.
- **GGUF** (GGML Unified Format) – designed for CPU inference, supports 2‑8 bits.
- **AWQ** – activation‑aware quantisation.

### Why quantise?
- **Run large models on small hardware** (e.g., Llama 70B on a single GPU).
- **Faster inference** (less memory bandwidth).
- **Lower energy consumption**.

### Quality impact
- 4‑bit quantisation typically loses <1% accuracy for generation tasks.
- 2‑bit degrades noticeably.

## 🛠️ Setup
```bash
pip install transformers accelerate bitsandbytes
# For GGUF: install llama-cpp-python