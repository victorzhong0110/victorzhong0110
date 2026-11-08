# Ideas

Raw theses before they become repos. Nothing here is measured. Each entry states what I believe, why, and what would change my mind. When an idea gets a working loop it moves to **Ideas → MVP** on the profile; when it gets a controlled result it moves to [research.md](research.md).

## 2026-11-08 · Kaggle 冠军工作流与自主问题发现型 ML Research Agent

**Observation.** 现有 MLE Agent 已能进行代码搜索、训练评估、迭代和部分自动特征工程，但高分不代表独立发现了数据生成机制、隐藏实体、恰当的验证体系或值得重构的中间任务。

**Thesis.** 在方案/代码实验图之外，显式维护“观察 → 竞争解释 → 鉴别实验 → 证据 → 问题重构”的假设证据图，可能让 AI 研究系统更接近顶尖 Kaggle 选手的研究能力，而不仅是更快地搜索模型。

**Test.** 在相同 LLM、工具和算力预算下，对比单 Agent、实验树、经验记忆、假设证据图、独立反证角色及元研究机制；用历史冠军案例加未公开的合成隐藏机制任务，分别评价最终成绩、发现质量、泄漏控制和发现成本。历史题目必须控制公开方案污染。

**What would change my mind.** 如果结构化解释层与反证机制在盲法实验中不能提升独立发现率，或其开销超过收益，则保留可执行实验/评测基础设施，删除额外多 Agent 与假设图复杂度。

**Full proposal.** [Kaggle champions vs autonomous ML research agents: workflows, problem discovery and benchmark design](ideas/2026-11-08-kaggle-research-agents-and-problem-discovery.md).

## 2026-11-08 · Adversarial, self-revising scientific agents — challenging the problem frame itself

**Observation.** LLM agents can optimize within a given hypothesis space while failing to challenge the space itself. Pro/con debate can strengthen shared biases; shared context may turn historical interpretations into unchallenged facts.

**Thesis.** Evidence-grounded falsification, independent reframing, and controlled meta-research may improve the ability to discover missing mechanisms and revise the research process itself. Fix the evidence protocol, not the roster of agents.

**Constraint that decides the design.** A system must not declare its own framework improved by rewriting its judge or reusing evaluation data. Keep raw evidence, competing interpretations, and task-specific context separate; test role structure and memory policy as variables. Compare against a strong single-agent baseline at matched experimental and compute cost.

**What would change my mind.** If independent holdouts show no improvement in discovering new causal/structural explanations, if multi-agent cost exceeds gains, or if alternative context policies do not reduce fixation, simplify or discard the architecture.

**Full research note:** [Adversarial self-revising scientific agents — fixation, falsification, memory, metaresearch](ideas/2026-11-08-adversarial-self-revising-science-agents.md).

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
