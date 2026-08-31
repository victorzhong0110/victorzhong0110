# Path and targets

This file is the shop-window rule for the **Open Source** column, not a list of my own repos.

## What recruiters should see there

Merged, reviewable PRs in a **living** LLM / agent codebase (post-training, agents, runtimes, eval). Star count on a solo repo does not count. A plugin that only I run does not count. Eval harness PRs are a way to get reviewed diffs; they are not a bid for an eval-only job.

## What exists today (2026-08)

| Kind | Status |
|---|---|
| Merged PR in a living post-training / agent repo | none yet |
| In flight | [inspect_evals#2320](https://github.com/UKGovernmentBEIS/inspect_evals/pull/2320) shortens duplicated Usage blocks ([#2253](https://github.com/UKGovernmentBEIS/inspect_evals/issues/2253)); not in the Open Source column until it merges |
| Listing in [Awesome DSH Plugin](https://github.com/xinglunxu76-star/awesome-dsh-plugin-deepseek-harness-/commit/18fac16c535225e72e187cdbf4d606bea01e6b2e) | one docs-list commit; too small to headline |

Personal tools ([skill-evolution](https://github.com/victorzhong0110/skill-evolution), [dsh-outcome-loop](https://github.com/victorzhong0110/dsh-outcome-loop), [dsh-code-reference](https://github.com/victorzhong0110/dsh-code-reference), [open-legal-aid](https://github.com/victorzhong0110/open-legal-aid), [llm-research-os](https://github.com/victorzhong0110/llm-research-os)) live under **Ideas → MVP** on the profile. They are how I ship loops. They are not community identity.

## What I will not do

- Another greenfield agent demo with a README full of logos.
- Website-only contributions to a famous foundation project just to put the logo on a resume.
- Join a 10-PR pile on a stale "good first issue" (Hendrycks `$` extraction, lighteval Count column, etc.).

## Where the real demand is (checked 2026-08-31)

Post-training trainers and agent runtimes that still merge tested diffs: TRL, PEFT, verl, SWIFT, LlamaFactory, Axolotl on the train/adapt side; DSPy, Pydantic AI, smolagents, SWE-agent, LangGraph, MCP Python SDK on the agent side.

Finish [inspect_evals#2320](https://github.com/UKGovernmentBEIS/inspect_evals/pull/2320) because it is already open. Do **not** open lm-eval or another eval-suite PR as the next identity move.

Operating rule: 1 merged PR in someone else's repo per month, starting 2026-09. If a project does not respond in two weeks, switch.

The active queue is 12 repos, post-training and agents (six each). Queue and calendar are tracked privately; a box is checked only after merge. Parallel in-flight PRs are allowed.
