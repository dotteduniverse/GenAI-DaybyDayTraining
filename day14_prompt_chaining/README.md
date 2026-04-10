# Day 14 – Prompt Chaining & Self‑Consistency

## 🎯 Learning Objectives
- Understand prompt chaining: breaking complex tasks into steps.
- Implement a multi‑step reasoning chain (e.g., extract → summarise → answer).
- Use self‑consistency: sample multiple reasoning paths and vote.

## 📚 Detailed Concepts

### Prompt Chaining
Instead of asking an LLM to do everything in one prompt, break the task into sub‑tasks, each with its own prompt.  
Example: Given a long email, you might:
1. Extract action items.
2. Summarise the tone.
3. Draft a reply.

**Advantages**:  
- Each step is simpler, less error‑prone.  
- Intermediate outputs can be inspected.  
- Easy to swap or improve individual steps.

### Self‑Consistency
For reasoning tasks (especially math or logic), ask the LLM to generate **multiple independent reasoning chains** (e.g., 5 times with temperature >0), then take the majority answer.  
Dramatically improves accuracy on tasks like GSM8K.

### Implementation patterns
- **Sequential chain**: output of step 1 → input of step 2.
- **Parallel chain**: run multiple prompts independently, then aggregate.
- **Conditional chain**: branch based on intermediate result.

## 🛠️ Setup
```bash
pip install openai langchain