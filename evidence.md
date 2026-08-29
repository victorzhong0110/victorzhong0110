# 📏 How to read claims

This profile is an evidence index, not a highlight reel. If a number cannot be regenerated from a public repo, it does not belong on the front page.

## Rules

1. **Product is the measurement.** A demo without a grader, a null, or a dispute log is a toy. Those stay in Ideas → MVP, not in the Open Source column.
2. **Nulls are first-class.** C1 self-verification moving accuracy by 0.0% is a result. Hiding it would be the actual failure.
3. **Artifacts are named.** Rate-limit collapse, partial-answer override, non-reproducible gold — they stay in the write-up.
4. **M0 is M0.** `llm-research-os` does not train, does not touch real GPUs, and `ready` on a dry-run is not “the experiment worked.”
5. **Internships are not invented.** This account has no ByteDance / Bilibili / Apache committer line. That gap is in [plan.md](plan.md), not papered over.

## What is independently checkable

| Claim | Where |
|---|---|
| da-verify C0/C1/C2/C3 numbers | [`da-verify` README + `report/report.md`](https://github.com/victorzhong0110/da-verify) |
| skill-evolution on PyPI | [pypi.org/project/skill-evolution](https://pypi.org/project/skill-evolution) |
| dsh-code-reference tests / policy / threat model | repo CI, `SECURITY.md`, 84 node:test cases |
| dsh-outcome-loop verification axes | `ARCHITECTURE.md`, 151 tests, coverage thresholds in CI |
| llm-research-os M0 scope | `docs/charter-v0.1.md`, threat model, schemas |
| Awesome DSH listing | [PR to awesome-dsh-plugin](https://github.com/xinglunxu76-star/awesome-dsh-plugin-deepseek-harness-/commit/18fac16c535225e72e187cdbf4d606bea01e6b2e) |

## What is not a claim yet

- Chaos constructions: written, not published. Do not cite as a paper.
- ArkNarrator: LoRA + LLM-as-judge on a small set. Useful as a lineage for da-verify, not as a production system.
- Course / visualization / gacha repos: archived or not pinned. They are learning residue.

## Voice

I would rather lose a bullet on a resume than keep a number that only survives because the ruler was buggy. That is the whole point of this library.
