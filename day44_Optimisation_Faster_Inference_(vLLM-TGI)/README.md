# Day 44: Optimisation – Faster Inference (vLLM, TGI)

## Learning Goals
- Understand techniques to speed up LLM inference: continuous batching, PagedAttention, kernel fusion.
- Deploy a model using vLLM for high‑throughput serving.
- (Optional) Use Hugging Face Text Generation Inference (TGI) for production.

## Topics Covered
1. Why optimisation matters: latency, throughput, cost.
2. vLLM: PagedAttention, continuous batching, support for many models.
3. Running a vLLM server and sending requests.
4. TGI: another production‑grade serving solution.

## Setup
```bash
# vLLM requires CUDA and specific PyTorch versions
pip install vllm

# TGI (optional) – best used via Docker
docker run --gpus all -p 8080:80 ghcr.io/huggingface/text-generation-inference:latest