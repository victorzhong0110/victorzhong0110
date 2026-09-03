# Path and targets

This file is the shop-window rule for the **Open Source** column, not a list of my own repos.

## What recruiters should see there

Merged, reviewable PRs in a **living** LLM / agent codebase (post-training, agents, runtimes, eval). Star count on a solo repo does not count. A plugin that only I run does not count. Eval harness PRs are a way to get reviewed diffs; they are not a bid for an eval-only job.

## What exists today (2026-09-03)

| Kind | Status |
|---|---|
| Merged PR in a living LLM / agent repo | [inspect_evals#2320](https://github.com/UKGovernmentBEIS/inspect_evals/pull/2320) merged 2026-09-01. Docs/tooling (Usage dedup, closes [#2253](https://github.com/UKGovernmentBEIS/inspect_evals/issues/2253)). Counts as a reviewed diff, not an eval-only bid. |
| In flight | [peft#3647](https://github.com/huggingface/peft/pull/3647) (post-training, empty adapter path). [pydantic-ai#8012](https://github.com/pydantic/pydantic-ai/pull/8012) (agents, TestModel formats). [inspect_evals#2324](https://github.com/UKGovernmentBEIS/inspect_evals/pull/2324) (register da-verify; C0 logs uploaded 2026-08-30, awaiting maintainer). huggingface/trl stays next in the queue, not a fourth parallel PR this week. |
| Listing in [Awesome DSH Plugin](https://github.com/xinglunxu76-star/awesome-dsh-plugin-deepseek-harness-/commit/18fac16c535225e72e187cdbf4d606bea01e6b2e) | one docs-list commit; too small to headline |

Personal tools ([skill-evolution](https://github.com/victorzhong0110/skill-evolution), [dsh-outcome-loop](https://github.com/victorzhong0110/dsh-outcome-loop), [dsh-code-reference](https://github.com/victorzhong0110/dsh-code-reference), [open-legal-aid](https://github.com/victorzhong0110/open-legal-aid), [llm-research-os](https://github.com/victorzhong0110/llm-research-os)) live under **Ideas → MVP** on the profile. They are how I ship loops. They are not community identity.

## What I will not do

- Another greenfield agent demo with a README full of logos.
- Website-only contributions to a famous foundation project just to put the logo on a resume.
- Join a 10-PR pile on a stale "good first issue" (Hendrycks `$` extraction, lighteval Count column, etc.).

## Where the real demand is (checked 2026-08-31)

Post-training trainers and agent runtimes that still merge tested diffs: TRL, PEFT, verl, SWIFT, LlamaFactory, Axolotl on the train/adapt side; DSPy, Pydantic AI, smolagents, SWE-agent, LangGraph, MCP Python SDK on the agent side.

[inspect_evals#2320](https://github.com/UKGovernmentBEIS/inspect_evals/pull/2320) merged 2026-09-01. September in-flight is peft + pydantic-ai + the da-verify register. huggingface/trl is next after those land. Do **not** open lm-eval as the next PR.

Operating rule: 1 merged PR in someone else's repo per month, starting 2026-09. If a project does not respond in two weeks, switch.

The active queue is 12 repos, post-training and agents (six each). Queue and calendar are tracked privately; a box is checked only after merge. Parallel in-flight PRs are allowed.
