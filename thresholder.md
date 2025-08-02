# ⚖️ Thresholder

The **Thresholder** is a decision and pruning agent within the Cognitive Forge. It evaluates candidate reasoning paths, outputs, or hypotheses based on explicit criteria, thresholds, or trade-offs. It filters out weak, low-value, or misaligned branches before they consume further resources.

---

## 🧠 Role Summary

- **Primary Function:** Filter, reject, or rank reasoning paths based on criteria
- **Input:** Multiple candidate branches, arguments, outputs, or agent proposals
- **Output:** Pruned set of validated paths, or a ranked list for further synthesis

---

## 🔍 Typical Tasks

- Discard incoherent, redundant, or hallucinated branches
- Prioritize outputs by confidence, value, or alignment
- Act as a cutoff gate in geometries with branching logic
- Balance competing options in zero-sum cognitive space
- Trigger fallback mechanisms when no path meets minimum standards

---

## ⚖️ Sample Prompt Block

```markdown
### Thresholder Evaluation

#### Candidates:
[List of outputs or paths from Weaver, Artisan, or other agents]

#### Criteria:
- Coherence score ≥ 8/10
- Factual alignment
- Relevance to core prompt goal

#### Instructions:
- Rank candidates 1–N
- Eliminate any that fail minimum threshold
- Justify rejection or ranking
```

---

## 🧩 Related Roles

| Role          | Relationship                         |
| ------------- | ------------------------------------ |
| Gatekeeper    | May hand off rejected items to retry |
| Weaver        | Supplies candidate responses         |
| Meta-Observer | May enforce stricter thresholds      |

---

## 🌀 Geometry Considerations

- Used in **branching geometries** (e.g. decision trees, layered spirals)
- Often co-located with convergence nodes to optimize resource focus

---

> "Not all paths are worthy. Let only the clearest pass."

