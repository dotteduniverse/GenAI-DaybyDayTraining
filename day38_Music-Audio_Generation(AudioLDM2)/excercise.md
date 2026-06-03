# Exercises – Day 38

1. **Different music genres**  
   Generate 5‑second clips for “jazz saxophone solo”, “electronic dance beat”, “orchestral string quartet”. Compare the outputs.

2. **Adjust guidance scale**  
   Keep the same prompt (“happy ukulele”) and vary `guidance_scale` from 1.0 to 4.0. Describe how adherence vs. creativity changes.

3. **Negative prompt effect**  
   Generate with prompt “rock guitar riff” and negative prompt “drums, bass”. Does it reduce drum presence? Try with/without negative.

4. **Longer generation**  
   Increase `audio_length_in_s` to 12 seconds. Does the quality degrade? Why might that happen?

5. **Bonus: Conditioning on a reference audio**  
   AudioLDM 2 can also be conditioned on an audio input. Read the docs and try generating a variation of an existing short audio clip.