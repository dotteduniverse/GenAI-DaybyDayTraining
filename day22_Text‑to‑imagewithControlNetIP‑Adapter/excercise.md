# Exercises – Day 22

1. **Sketch from real photo**  
   Take any photo (e.g., a dog, a house). Use Canny edge detection to extract an edge map. Use that edge map as control input with a text prompt (“a photo of a house”, etc.). Compare output with and without ControlNet.

2. **Different ControlNet types**  
   Replace the Canny ControlNet with a different one: `lllyasviel/sd-controlnet-scribble` or `lllyasviel/sd-controlnet-depth`. Test the same sketch. How does output change?

3. **Control strength**  
   Experiment with `controlnet_conditioning_scale` from 0.0 to 1.5. Describe what happens at low (0.2) vs high (1.2) values.

4. **Hand‑drawn sketch**  
   Draw a simple sketch on paper, photograph it, convert to edges, and use as control. Does the model follow your drawing?

5. **Bonus: IP‑Adapter**  
   Install `ip-adapter` from [GitHub](https://github.com/tencent-ailab/IP-Adapter). Use a reference image (e.g., a painting style) and generate a new image of a cat in that style. Combine IP‑Adapter with ControlNet if possible.