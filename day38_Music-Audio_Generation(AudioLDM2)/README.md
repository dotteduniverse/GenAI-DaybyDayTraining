# Day 38: Music & Audio Generation (AudioLDM 2)

## Learning Goals
- Understand text‑to‑audio generation using latent diffusion models.
- Use AudioLDM 2 to generate short music clips, sound effects, or speech from text prompts.
- Save and listen to generated audio.

## Topics Covered
1. Loading AudioLDM 2 pipeline from Hugging Face Diffusers.
2. Generating audio from a text prompt.
3. Adjusting parameters: duration, guidance scale, number of inference steps.
4. Saving as .wav file and playing in notebook.

## Setup
```bash
pip install diffusers transformers accelerate audioldm2 soundfile torchaudio