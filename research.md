# Research

## 1. da-verify — verification is variance reduction, not capability injection

Repo: [victorzhong0110/da-verify](https://github.com/victorzhong0110/da-verify)

**Question.** On data-analysis tasks whose answers can be checked by a program: how much does adding verification raise success rate, and at what cost?

**Design.** Same model, harness, 40-task subset, and grader. Conditions differ only in the verification policy.

| Condition | What it is | Headline |
|---|---|---|
| C0 | ReAct, no verification | temp 0: 82.5% pass@1; temp 0.7 k=5: 64.5% |
| C1 | same-model self-check | Δ 0.0% — clean null |
| C2 | independent LLM re-derivation | +11.0 pt pass@1 at temp 0.7 / k=5; invisible at temp 0 / k=1 |
| C3 | self-consistency + programmatic agreement | pass@1 84.5%; vs C0 Δ +20.0 pt, CI [+10.5, +30.0] |

**Claim I will defend in an interview.** The active ingredient is sample diversity plus programmatic reconciliation — not LLM judgment. Failures land where the theory says they must: non-reproducible gold, and confident-wrong systematic errors.

**What I will not say.** That verification “makes the agent smarter.” At temp 0 there is no variance to repair.

Lineage: upgrades the eval harness from [ArkNarrator](https://github.com/victorzhong0110/ark-narrator) (Qwen2.5-7B / Qwen3-8B LoRA, DeepSeek V4 Pro judge, attribution / contradiction / pairwise). ArkNarrator is the ancestor, not the flagship.

## 2. llm-research-os — independent research IR, M0 only

Repo: [victorzhong0110/llm-research-os](https://github.com/victorzhong0110/llm-research-os)

A model-agnostic, backend-agnostic research OS: express a problem, compose blocks, let an AI propose and object, execute on local or remote workers, record training / eval / cost / lineage / AI decisions.

**Current honest status.** Charter v0.1 accepted. M0 = ResearchSpec protocol, versioned JSON Schema, validator, CloudEvents-compatible `ResearchEvent`, static dry-run kernel. It does **not** import block entry points, does **not** run training, and does **not** spend GPU. `ready` means the spec and static plan are complete — not that science happened.

This is the long-horizon original work. It is not a 2026 autumn-recruit resume bullet until a worker actually runs a bounded experiment with an event log.

## 3. Chaos maps — constructions, proofs, self-attack

Independent work on multi-valued / coupled chaotic maps (nD-MVC / CnD-MVC line): constructions, proofs, finite-precision notes.

**Working standard.** If I can mount an equal-cost attack on my own scheme, the claim is downgraded in public, not patched in the abstract. That is the same honesty rule as da-verify’s dispute log.

**Status.** In progress. Not a publication. Not listed as “papers” on the profile until there is a preprint with a stable claim.

## 4. Adjacent measurement work (not headline)

- [olist-commerce-analytics](https://github.com/victorzhong0110/olist-commerce-analytics) — SQL metrics → PSM / E-value → A/B design. Rigor-first course-scale study.
- [open-legal-aid](https://github.com/victorzhong0110/open-legal-aid) — RAG recall@k / MRR / refusal; rerank helps, local-small-model query rewrite does not. 25-item eval set, numbers in-repo.
