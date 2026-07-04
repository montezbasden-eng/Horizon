---
layout: default
title: "Horizon Summary: 2026-07-04 (EN)"
date: 2026-07-04
lang: en
---

> From 46 items, 5 important content pieces were selected

---

1. [Mistral Releases Leanstral-1.5: 6B Active Parameter Model for Formal Verification](#item-1) ⭐️ 9.0/10
2. [Soatok's Sassy Guide to Threat Modeling](#item-2) ⭐️ 8.0/10
3. [CVE Severity Spike Linked to Claude Mythos Preview](#item-3) ⭐️ 8.0/10
4. [Open Source AI Gap Map Launched](#item-4) ⭐️ 8.0/10
5. [Course Creator Reports 50%+ Sales Drop Due to AI](#item-5) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Mistral Releases Leanstral-1.5: 6B Active Parameter Model for Formal Verification](https://www.reddit.com/r/LocalLLaMA/comments/1umgdhx/mistral_released_leanstral15119ba6b/) ⭐️ 9.0/10

Mistral has released Leanstral-1.5, a 119B total parameter model with 6B active parameters, achieving state-of-the-art results on formal verification benchmarks including miniF2F, PutnamBench, FATE-H, and FATE-X. The model discovered 5 previously unknown bugs across 57 real-world repositories. This release demonstrates that small, efficient models can achieve competitive or superior performance in specialized domains like formal verification, making advanced AI capabilities more accessible and cost-effective. It also highlights the potential of AI to improve software reliability by automatically finding bugs that traditional testing misses. Leanstral-1.5 is trained using mid-training, supervised fine-tuning, and reinforcement learning with CISPO (Clipped Importance Sampling Policy Optimization). It is released under the Apache-2.0 license, enabling broad use and modification.

reddit · r/LocalLLaMA · /u/Tall-Ad-7742 · Jul 3, 14:44

**Background**: Formal verification uses mathematical proofs to guarantee software correctness, but traditionally requires significant human expertise. AI models like Leanstral-1.5 aim to automate this process by generating proofs or finding bugs in code. Benchmarks like miniF2F and PutnamBench test models on mathematical theorem proving, while FATE-H and FATE-X evaluate real-world code verification.

<details><summary>References</summary>
<ul>
<li><a href="https://www.emergentmind.com/topics/cispo-algorithm">CISPO: Clipped Importance Sampling RL - emergentmind.com</a></li>
<li><a href="https://arxiv.org/pdf/2109.00110">Formal o lympiad - level</a></li>
<li><a href="https://trishullab.github.io/PutnamBench/">PutnamBench : A Multilingual Mathematics Benchmark for Formal...</a></li>

</ul>
</details>

**Discussion**: Community comments show mixed reactions: some praise Mistral's focus on small, efficient models for specific tasks, while others criticize the benchmark comparisons as outdated. There is also discussion about the bug-finding example, with some questioning whether the discovered bug was truly hard to find via traditional testing.

**Tags**: `#AI`, `#formal verification`, `#Mistral`, `#open-source`, `#theorem proving`

---

<a id="item-2"></a>
## [Soatok's Sassy Guide to Threat Modeling](https://soatok.blog/2026/06/30/soatoks-informal-guide-to-threat-models/) ⭐️ 8.0/10

Soatok published an informal, sassy guide to threat modeling that emphasizes making assumptions explicit and defining adversaries and assets before assessing security. This guide helps security practitioners move beyond compliance checklists and think critically about what 'secure' actually means in their context, improving real-world security posture. The guide uses an end-to-end encryption example to illustrate threat modeling concepts, and it highlights that 'secure' is meaningless without specifying the adversary and assets.

hackernews · zdw · Jul 4, 00:35 · [Discussion](https://news.ycombinator.com/item?id=48781597)

**Background**: Threat modeling is a structured approach to identifying and prioritizing potential threats to a system. It typically involves defining assets, adversaries, and trust boundaries, then analyzing attack vectors. Soatok's guide presents this in a humorous, accessible style.

**Discussion**: Commenters praised the guide for its humor and clarity, with one noting it makes assumptions explicit rather than being a compliance checklist. Another raised the challenge of keeping threat models current as systems evolve, and a discussion on quantum computing scenarios emerged.

**Tags**: `#threat modeling`, `#security`, `#cryptography`, `#privacy`

---

<a id="item-3"></a>
## [CVE Severity Spike Linked to Claude Mythos Preview](https://epoch.ai/data-insights/cve-severity-spike) ⭐️ 8.0/10

In June 2026, 21 notable organizations disclosed around 1,500 high- and critical-severity CVEs, a 3.5× increase over the previous monthly record set before the release of Claude Mythos Preview. This spike suggests AI-assisted vulnerability discovery is accelerating, raising concerns about software security and the potential for AI to both find and exploit vulnerabilities at scale. The data comes from Epoch AI, which tracked CVEs from notable organizations. The increase is particularly pronounced for high- and critical-severity vulnerabilities, and the timing correlates with the release of Claude Mythos Preview.

hackernews · cubefox · Jul 3, 21:16 · [Discussion](https://news.ycombinator.com/item?id=48780056)

**Background**: Claude Mythos Preview is a large language model developed by Anthropic, announced on April 7, 2026. It has not been publicly released due to safety concerns over its ability to find software vulnerabilities. CVEs (Common Vulnerabilities and Exposures) are publicly disclosed security flaws.

<details><summary>References</summary>
<ul>
<li><a href="https://epoch.ai/data-insights/cve-severity-spike">Disclosed CVEs : 3.5× Spike After Claude Mythos | Epoch AI</a></li>
<li><a href="https://en.wikipedia.org/wiki/Claude_Mythos_Preview">Claude Mythos Preview</a></li>
<li><a href="https://digg.com/tech/4imbgb1q">Epoch AI reports CVE disclosures surged 3.5x to a record 1,500 in...</a></li>

</ul>
</details>

**Discussion**: Community comments express mixed views: some argue the spike was expected and not news, while others debate whether the reports are valid or could include hallucinations. Some attribute the increase to wider AI tool adoption rather than Mythos specifically.

**Tags**: `#AI security`, `#vulnerabilities`, `#Claude Mythos`, `#CVE`, `#software quality`

---

<a id="item-4"></a>
## [Open Source AI Gap Map Launched](https://simonwillison.net/2026/Jul/3/open-source-ai-gap-map/#atom-everything) ⭐️ 8.0/10

Current AI, a non-profit founded in February 2025 with $400M in committed capital, launched the Open Source AI Gap Map v0.1, indexing 421 products across the AI stack, including 266 software tools, 85 models, 50 datasets, and 20 hardware projects. This map provides a structured overview of the open source AI ecosystem, helping researchers and practitioners identify gaps and prioritize investments, which is crucial for advancing open source AI. The underlying data is released under an MIT license on GitHub, containing 1,184 YAML files and scripts, and the project tracks 16,185 GitHub repos, which can be explored via Datasette Lite.

rss · Simon Willison · Jul 3, 22:04

**Background**: The AI stack typically consists of multiple layers, such as model components, product/UX, and infrastructure. Open source AI projects span these layers, but gaps exist where proprietary solutions dominate. Current AI's Gap Map aims to systematically identify these gaps to guide development and funding.

<details><summary>References</summary>
<ul>
<li><a href="https://simonwillison.net/2026/Jul/3/open-source-ai-gap-map/">Open Source AI Gap Map - simonwillison.net</a></li>
<li><a href="https://map.currentai.org/">Current AI – Open Source AI Gap Map</a></li>
<li><a href="https://www.currentai.org/blogs/introducing-the-gap-map-v0-1">Introducing the Gap Map v0.1 - currentai.org</a></li>

</ul>
</details>

**Tags**: `#open source`, `#AI`, `#ecosystem mapping`, `#non-profit`

---

<a id="item-5"></a>
## [Course Creator Reports 50%+ Sales Drop Due to AI](https://simonwillison.net/2026/Jul/3/josh-w-comeau/#atom-everything) ⭐️ 8.0/10

Josh W. Comeau, a course creator, reported that his third course launch sold about one-third as many copies as typical, and his existing courses saw sales down significantly from last year, attributing the decline to AI-driven uncertainty about developer jobs and LLMs replacing paid educational content. This firsthand data from a prominent course creator highlights a tangible economic impact of AI on developer education, potentially signaling a broader trend that could reshape the online learning industry and affect many educators and learners. Comeau noted a 'double whammy': people are reluctant to invest time and money in learning new dev skills due to job uncertainty, and LLMs provide personalized tutoring, reducing the incentive to buy paid courses. He also mentioned that other course creators are seeing the same trend, with revenue down 50%+.

rss · Simon Willison · Jul 3, 21:25

**Background**: Online courses for developers have been a popular way to learn new skills, with creators like Josh W. Comeau building businesses around premium content. The rise of large language models (LLMs) like GPT-4 and Claude has enabled AI to generate code explanations, tutorials, and even personalized tutoring, potentially competing with traditional paid courses. Additionally, widespread discussion about AI replacing developer jobs has created uncertainty in the job market, discouraging investment in learning.

<details><summary>References</summary>
<ul>
<li><a href="https://medium.com/@keshavarangarajan/the-impact-of-llms-on-learning-and-education-3cd2a8367c23">The Impact of LLMs on Learning and Education | by keshava rangarajan | Medium</a></li>
<li><a href="https://nationalcentreforai.jiscinvolve.org/wp/2025/08/07/how-to-choose-the-right-models-llms-in-education-explained/">How to Choose the Right Model: LLMs in Education Explained - Artificial intelligence</a></li>
<li><a href="https://www.thirdrocktechkno.com/blog/llm-based-tutors/">Can AI Really Replace Teachers? LLMs in Education | 2026</a></li>

</ul>
</details>

**Tags**: `#AI impact`, `#developer education`, `#online courses`, `#job market`, `#LLMs`

---