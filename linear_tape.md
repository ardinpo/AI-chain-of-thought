# 📼 Linear Tape Geometry

The **Linear Tape** is the simplest geometry in the Cognitive Forge. It models reasoning as a left-to-right sequence with memory decay, much like a traditional prompt history. Each step builds on the last, but information naturally degrades over time unless reinforced.

This is the baseline memory model most LLMs use implicitly — but within the Forge, it can be formalized, monitored, and optionally extended.

---

## 🧠 Purpose

- Simulate classical step-by-step reasoning
- Emphasize temporal continuity and recency bias
- Provide a controlled decay model for short- to mid-term memory

---

## 📼 Tape Dynamics

- Each "frame" is a time-ordered memory segment
- Older frames may be pruned or deprioritized
- Weaver can summarize past frames into shorter tokens
- Meta-Observer can trigger reinforcement if degradation is too high

---

## 🔁 Prompt Format Example

```markdown
### Linear Tape – Frame 4

#### Prior Frames:
1. Setup
2. Hypothesis
3. Agent Reasoning

#### Instructions:
- Continue from Frame 3
- Maintain context
- Do not re-summarize prior content unless asked
```

---

## 🧩 Ideal Use Cases

- Narrative construction
- Code walkthroughs
- Procedural logic or simulations
- Conversation logs and behavioral modeling

---

## ⚠️ Decay Notes

- High risk of forgetting key insights without compression or elevation
- Works best when paired with summarization agents or checkpoint frames
- Consider combining with `Torus Buffer` or `Fractal Archive` for memory hybridization

---

> “The tape moves forward, but only the sharpest signals endure.”

