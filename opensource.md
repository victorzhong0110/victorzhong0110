# Path and targets

This file is the shop-window rule for the **Open Source** column, not a list of my own repos.

## What recruiters should see there

Merged, reviewable PRs in a **living** eval / harness / agent-runtime codebase. Star count on a solo repo does not count. A plugin that only I run does not count.

## What exists today (2026-08)

| Kind | Status |
|---|---|
| Merged PR in Inspect / lm-eval / EvalScope / OpenCompass | none yet |
| In flight | [inspect_evals#2320](https://github.com/UKGovernmentBEIS/inspect_evals/pull/2320) shortens duplicated Usage blocks ([#2253](https://github.com/UKGovernmentBEIS/inspect_evals/issues/2253)); not in the Open Source column until it merges |
| Listing in [Awesome DSH Plugin](https://github.com/xinglunxu76-star/awesome-dsh-plugin-deepseek-harness-/commit/18fac16c535225e72e187cdbf4d606bea01e6b2e) | one docs-list commit; too small to headline |

Personal tools ([skill-evolution](https://github.com/victorzhong0110/skill-evolution), [dsh-outcome-loop](https://github.com/victorzhong0110/dsh-outcome-loop), [dsh-code-reference](https://github.com/victorzhong0110/dsh-code-reference), [open-legal-aid](https://github.com/victorzhong0110/open-legal-aid), [llm-research-os](https://github.com/victorzhong0110/llm-research-os)) live under **Ideas → MVP** on the profile. They are how I ship loops. They are not community identity.

## What I will not do

- Another greenfield agent demo with a README full of logos.
- Website-only contributions to a famous foundation project just to put the logo on a resume.
- Join a 10-PR pile on a stale "good first issue" (Hendrycks `$` extraction, lighteval Count column, etc.).

## Where the real demand is (checked 2026-08-29)

Living eval repos are full of **grader soundness** bugs: substring `yes`/`no` parsers, judge outages scored as success, pipeline failures marked INCORRECT. That is the same class of defect as da-verify. Many of those tickets already have a PR from the reporter.

Unclaimed maintainer-requested work that is still worth doing:

1. [inspect_evals#2253](https://github.com/UKGovernmentBEIS/inspect_evals/issues/2253) — shorten duplicated Usage blocks in generated eval READMEs.
2. [inspect_evals#2295](https://github.com/UKGovernmentBEIS/inspect_evals/issues/2295) — repo-wide OpenRouter quantization pinning linter (larger; collaborator wants provider pinning too).
3. Do **not** pile onto lm-eval#2552 or lighteval#804.

Operating rule: 1 merged PR in someone else's repo per month, starting 2026-09. If a project does not respond in two weeks, switch.

The active queue is [oss-todo.md](oss-todo.md): 12 repos, eval-heavy (eight harness/eval seats, then DSPy, LiteLLM, Pydantic AI, MCP Python SDK). The full 81-repo list stays in [oss-catalog.md](oss-catalog.md). Check a box only after merge. Parallel in-flight PRs are allowed.

Calendar: [plan.md](plan.md).
