# Exercises – Day 24

1. **Different input images**  
   Generate a short video from two different images: a portrait of a person and a abstract painting. Describe how the motion differs.

2. **Looping with cross‑fade**  
   Instead of simply reversing, create a smooth loop by blending the last frame into the first using a cross‑fade (e.g., 10 frames of linear interpolation). Save as a GIF.

3. **Frame rate experiment**  
   Generate the same video but export at different fps (5, 10, 15). Which looks most natural for the content?

4. **Motion bucket sweep**  
   Sweep `motion_bucket_id` from 20 to 200 in steps of 40. Generate videos and compare. What happens at extremely low or high values?

5. **Bonus: Text‑to‑video with SVD + prompt**  
   SVD is image‑to‑video only. Use a text‑to‑image model first (e.g., Stable Diffusion) to create a starting image, then feed it to SVD. Generate a video of “a dragon flying over a castle” using this two‑step process.