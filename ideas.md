# Ideas

Raw theses before they become repos. Nothing here is measured. Each entry states what I believe, why, and what would change my mind. When an idea gets a working loop it moves to **Ideas → MVP** on the profile; when it gets a controlled result it moves to [research.md](research.md).

## 2026-09-02 · Governed parameter evolution — an agent that cannot update its weights cannot correct itself

**Observation.** Harnesses and instruction files (AGENTS.md, skills, memory) edit the *context*, not the model. Whatever is corrected in conversation evaporates at session end. The model also has no provenance over its own knowledge: it cannot tell when a concept entered its parameters, so it cannot locate the part to revise. It treats the factory distribution as the prior of truth. In agents this reads as rigidity — it can accept your logic mid-conversation and still act from its training-set bias.

**Thesis.** The durable fix is parameter-level evolution driven by human interaction and self-reflection — not a bigger harness.

**Constraint that decides the design.** Current interpretability research is far too weak to guarantee surgical edits: we cannot yet correct the targeted behavior with confidence that core capabilities and unrelated capabilities stay intact. So near-term "evolution" must be coarse-grained (adapters, small bounded fine-tunes) wrapped in evaluation — not precise weight surgery. Anyone promising surgical correction today is overselling.

**Three tiers, three tools.**

- **Facts and preferences** → external memory / retrieval. Weights are not needed; using parameter updates for this tier actively harms generality.
- **Skills and behavior patterns** → weight-level intervention (adapters, preference-style post-training). The only tier where parameter evolution is irreplaceable.
- **Deep bias / "stereotypes"** → cannot be self-certified: the model grades its own correction with the pre-correction judge. Requires external evaluation and human approval. Pure self-loops fail in principle.

**Why this makes a control plane prerequisite, not optional.** Once weights evolve, every step is a governance question: who authorizes a self-modification (irreversible compared to prompts); how to roll back (content-addressed checkpoints); how to prove improvement (fixed eval suites, baselines, and "insufficient evidence" as an allowed verdict); whose interactions shaped the weights (lineage and consent). This is the long-horizon arc of [llm-research-os](https://github.com/victorzhong0110/llm-research-os): L0 record → L1 governed execution → L2 human-in-the-loop research → L3 governed parameter evolution / full-auto AI scientist.

**Risks on the record.** Catastrophic forgetting; alignment drift; reward hacking (learning to *look* corrected rather than be corrected); single-user bias capture (one person's interactions baked into weights); interpretability too weak for surgical edits (above).

**What would change my mind.** Evidence that external memory plus retrieval closes the behavior gap at parity with weight updates on skills; or interpretability maturing enough to make surgical, side-effect-free edits routine. Either would demote the governance-heavy path.
