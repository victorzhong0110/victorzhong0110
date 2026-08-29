# Projects

Pinned story, in order. Everything else is either M0, a lineage experiment, or learning residue.

## A. Agents that can be checked

### da-verify

Verification-in-the-loop data-analysis agent + evaluation harness. See [research.md](research.md).

**Why it is the flagship.** It has a thesis, a controlled comparison, a grader with a gold self-check, and published nulls. Interviewers can clone it.

### dsh-outcome-loop

[victorzhong0110/dsh-outcome-loop](https://github.com/victorzhong0110/dsh-outcome-loop)

DeepSeek Harness plugin: a local-first outcome ledger. Mechanical verification and user disposition are independent axes. Default cost is zero extra tokens. Unknown is never silently turned into success. Export is two-phase (preview digest → approve).

This is the engineering form of the same idea as da-verify: “the model said done” is not a result.

### skill-evolution

[victorzhong0110/skill-evolution](https://github.com/victorzhong0110/skill-evolution) · PyPI `skill-evolution`

Framework-agnostic CLI: evolve skill documents by comparing successful vs failed trajectories, then targeted patches, then an independent auditor. Inspired by SkillEvolver / EmbodiSkill; the product is the loop, not a paper replica.

## B. Harness plugins (distribution inside a real runtime)

### dsh-code-reference

[victorzhong0110/dsh-code-reference](https://github.com/victorzhong0110/dsh-code-reference)

Before writing new code: survey local + GitHub/npm, score reuse vs adapt vs dependency vs rewrite, **ask the user**. Architecture-level reuse is a candidate signal, not an auto-decision. Unknown licenses fail closed when a whitelist exists. Deploy-time policy is a ceiling the workspace cannot relax.

Listed in Awesome DSH Plugin. Status: reliable beta, not GA.

## C. Long-horizon original work

### llm-research-os

M0 protocol kernel. See [research.md](research.md). Do not describe this as a training platform yet.

## D. Applied systems (evidence exists, not the career headline)

| Repo | One line | Limit |
|---|---|---|
| [open-legal-aid](https://github.com/victorzhong0110/open-legal-aid) | Local RAG + citable statutes + Word filings | Not a licensed legal service; eval set is small |
| [ark-narrator](https://github.com/victorzhong0110/ark-narrator) | LoRA roleplay + judge eval | Small eval; ancestor of da-verify |
| [olist-commerce-analytics](https://github.com/victorzhong0110/olist-commerce-analytics) | Causal / experiment design on Olist | Course-scale |

## E. Not on the shop window

Course homework, early visualization, archived price/wordcloud repos, and Universe City design notes stay unpinned. They are how I learned; they are not how I want to be hired.

If a recruiter only has 90 seconds: **da-verify**. Personal plugins belong under Ideas → MVP on the profile, not in the Open Source column.
