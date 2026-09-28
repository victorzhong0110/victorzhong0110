<div align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Cascadia+Code&weight=700&size=22&duration=2000&pause=100000&color=0078D7&center=true&vCenter=true&repeat=false&width=280&height=45&lines=I%27m%20Vic." alt="I'm Vic." />
  <br/>
  <img src="./assets/tagline-light.svg#gh-light-mode-only" alt="LLM research · post-training · agents" />
  <img src="./assets/tagline-dark.svg#gh-dark-mode-only" alt="LLM research · post-training · agents" />
  <p>
    <code>Born in 2005 · Zhejiang, China.</code>
    <code>Now based in Shanghai.</code>
  </p>
  <p>
    Hugging Face: <a href="https://huggingface.co/victorzhong">victorzhong</a>
  </p>
</div>

<table>
<tr>
<td valign="top" width="34%">

#### Research

> [How to read claims →](evidence.md)

<p>
<strong><a href="https://github.com/victorzhong0110/da-verify">da-verify</a></strong> -- <code>C0/C1/C2/C3 · programmatic agreement</code> -- <code>flagship</code>
</p>

Verification on data-analysis agents repairs variance, not capability. C1 is a clean null. The active ingredient is sample diversity plus a programmatic grader.

</td>
<td valign="top" width="33%">

#### Open Source

> [Path & targets →](opensource.md)

Merged work in **other people's** LLM / agent codebases. Personal plugins do not go here.

<p>
<strong><a href="https://github.com/UKGovernmentBEIS/inspect_evals/pull/2320">inspect_evals#2320</a></strong> -- <code>docs · Usage dedup</code> -- <code>merged 2026-09-01</code>
</p>
<p>
<strong><a href="https://github.com/huggingface/peft/pull/3647">peft#3647</a></strong> -- <code>empty adapter path on save</code> -- <code>merged 2026-09-04</code>
</p>

Two merged PRs. In flight includes pytorch/pytorch. New Hugging Face first cuts paused 2026-09-06.

</td>
<td valign="top" width="33%">

#### Now

In-flight only. A result moves left when it is merged or measured.

- **Focus: [llm-research-os](https://github.com/victorzhong0110/llm-research-os)** — research control plane · M2 local/two-host accepted ([ADR-0062](https://github.com/victorzhong0110/llm-research-os/blob/main/docs/adr/0062-m1-m2-acceptance-and-m3-boundary.md)) · laptop CUDA 20-step LoRA + checkpoint-10→12 restore · paid cloud not run · M3 in progress: R01–R03 accepted, [R04](https://github.com/victorzhong0110/llm-research-os/pull/111) merged 2026-09-28 (runtime prep; launch still refused) · Public MVP not released · <code>2026-09</code>
- **[pytorch#196017](https://github.com/pytorch/pytorch/pull/196017)** — prune.remove parameter order · `in review` · Individual CLA signed · <code>2026-09</code>
- **[pydantic-ai#8012](https://github.com/pydantic/pydantic-ai/pull/8012)** — TestModel datetime / UUID / URI · `open` · <code>2026-09</code>
- **[inspect_evals#2324](https://github.com/UKGovernmentBEIS/inspect_evals/pull/2324)** — register da-verify · logs uploaded, awaiting maintainer · <code>2026-08</code>
- Internships in LLM / post-training / agents · Shanghai · 2027

</td>
</tr>
</table>

#### Ideas → MVP

> [Raw theses before they become repos →](ideas.md)

I like taking a precise idea to a working loop quickly. These are **not** community products; they show how I spec, ship, and measure a small system.

| Project | What it proves | Status |
|---|---|---|
| **[skill-evolution](https://github.com/victorzhong0110/skill-evolution)** | Framework-agnostic CLI: evolve skill docs from successful vs failed trajectories, targeted patches, independent auditor | [![PyPI](https://img.shields.io/pypi/v/skill-evolution?style=flat-square&color=0078D7)](https://pypi.org/project/skill-evolution) |
| **[open-legal-aid](https://github.com/victorzhong0110/open-legal-aid)** | Local RAG for Chinese legal self-help: citable statutes + Word filings | Rerank helps; query-rewrite ablation negative (25-item eval) |
| **[llm-research-os](https://github.com/victorzhong0110/llm-research-os)** | Model-agnostic research OS: express a problem, compose blocks, record lineage and AI decisions | M2 local/two-host accepted · laptop CUDA live · M3 through R04 merged, launch still refused · paid cloud not run · Public MVP not released |
