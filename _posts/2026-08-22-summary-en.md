---
layout: default
title: "Horizon Summary: 2026-08-22 (EN)"
date: 2026-08-22
lang: en
---

> From 43 items, 4 important content pieces were selected

---

1. [NVIDIA AVO Scores Perfect 100% on ARC-AGI-3 Benchmark](#item-1) ⭐️ 9.0/10
2. [Scientists Release Largest 2D Map of the Universe](#item-2) ⭐️ 8.0/10
3. [Researcher Accidentally Hijacks e164.arpa DNS, Logging Military Calls](#item-3) ⭐️ 8.0/10
4. [Stop Making TUIs: Build Native UIs with AI Agents](#item-4) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [NVIDIA AVO Scores Perfect 100% on ARC-AGI-3 Benchmark](https://www.reddit.com/r/LocalLLaMA/comments/1vuh7to/nvidia_avo_got_100_on_arcagi3_it_completed_all/) ⭐️ 9.0/10

NVIDIA's AVO agent system achieved a perfect score of 100% on the ARC-AGI-3 benchmark, completing all 183 levels across 25 public environments without any instructions, explicit rules, or stated goals. This marks a significant leap from the previous best single-model score of around 30%. This achievement demonstrates a frontier-level general-purpose architecture for long-horizon autonomous agents, suggesting progress toward artificial general intelligence (AGI). It could reshape expectations for AI capabilities in novel, interactive environments and influence future benchmark design and agent development. AVO is a general-purpose coding agent system developed by NVIDIA, capable of inspecting and editing code, running commands, consulting documentation, and validating its actions. It reportedly achieved 1668 TFLOPS and transferred optimizations between tasks in just 30 minutes, highlighting its efficiency and adaptability.

reddit · r/LocalLLaMA · /u/theologi · Aug 21, 14:01

**Background**: ARC-AGI-3 is the first interactive reasoning benchmark in the ARC-AGI series, designed to evaluate agentic intelligence through novel, abstract, turn-based environments. Unlike its predecessors, it requires agents to explore, infer goals, build internal models of environment dynamics, and plan actions without explicit instructions. The benchmark is part of the Abstraction and Reasoning Corpus (ARC) family, which focuses on fluid adaptive efficiency.

<details><summary>References</summary>
<ul>
<li><a href="https://developer.nvidia.com/blog/nvidia-avo-reaches-100-on-arc-agi-3-demonstrating-a-frontier-level-general-purpose-architecture-for-long-horizon-autonomous-agents/">NVIDIA AVO Reaches 100% on ARC-AGI-3, Demonstrating...</a></li>
<li><a href="https://arcprize.org/arc-agi/3">ARC-AGI-3</a></li>
<li><a href="https://arxiv.org/abs/2603.24621">ARC-AGI-3: A New Challenge for Frontier Agentic Intelligence Announcing ARC-AGI-3 - ARC Prize ARC-AGI-3: A New Challenge for Frontier Agentic Intelligence ARC-AGI-3 Leaderboard - llm-stats.com How enabling two settings tripled our scores on the ARC-AGI-3 ...</a></li>

</ul>
</details>

**Discussion**: The Reddit community expressed excitement and skepticism, with many praising NVIDIA's achievement as a major milestone while others questioned the benchmark's validity and whether AVO's success truly indicates AGI. Some users noted the lack of transparency in AVO's methodology and called for independent verification.

**Tags**: `#AI`, `#AGI`, `#NVIDIA`, `#ARC-AGI`, `#Benchmark`

---

<a id="item-2"></a>
## [Scientists Release Largest 2D Map of the Universe](https://newscenter.lbl.gov/2026/08/10/scientists-release-biggest-2d-map-of-the-universe/) ⭐️ 8.0/10

Scientists have released the largest two-dimensional map of the universe, created from the DESI Legacy Imaging Surveys, which combined over 263,000 telescope exposures. The map includes nearly 4 billion celestial objects and is available through an interactive viewer at viewer.legacysurvey.org. This map provides an unprecedented comprehensive view of the universe, enabling astronomers to study large-scale structures and search for rare phenomena. It is expected to remain the most comprehensive 2D map for years, serving as a foundational resource for future astronomical research. The map covers roughly three-quarters of the sky and contains about 5.6 trillion pixels. It combines visible and near-infrared light data, and the interactive viewer allows users to explore the sky and zoom into specific regions.

hackernews · NKosmatos · Aug 21, 18:36 · [Discussion](https://news.ycombinator.com/item?id=49392200)

**Background**: The DESI Legacy Imaging Surveys are a series of ground-based surveys that have mapped the sky in multiple wavelengths. The resulting map is a mosaic of images that astronomers can use to identify galaxies, quasars, and other objects, and to plan follow-up observations with other telescopes.

<details><summary>References</summary>
<ul>
<li><a href="https://newscenter.lbl.gov/2026/08/10/scientists-release-biggest-2d-map-of-the-universe/">Scientists Release Biggest 2D Map of the Universe</a></li>
<li><a href="https://www.space.com/astronomy/scientists-create-largest-2d-map-of-the-universe-with-5-6-trillion-pixels-and-nearly-4-billion-cosmic-objects">Scientists create largest 2D map of the universe with 5.6 ...</a></li>
<li><a href="https://www.independent.co.uk/space/astronomy-two-dimensional-map-universe-scientists-b3031325.html">Scientists just released the biggest two-dimensional map of ...</a></li>

</ul>
</details>

**Discussion**: Community comments express awe at the map's scale and detail, with some users sharing specific coordinates to explore. There is also discussion about the possibility of a 3D map and the computational challenges involved, as well as skepticism about future investment in astronomy given economic and strategic priorities.

**Tags**: `#astronomy`, `#science`, `#data visualization`, `#universe mapping`

---

<a id="item-3"></a>
## [Researcher Accidentally Hijacks e164.arpa DNS, Logging Military Calls](https://lina.sh/blog/hijacking-e164-arpa) ⭐️ 8.0/10

A security researcher accidentally hijacked DNS queries for the e164.arpa domain, logging hundreds of thousands of phone calls, including those to military bases. The incident was detailed in a blog post that highlights a critical but overlooked infrastructure flaw. This incident exposes a significant vulnerability in the e164.arpa infrastructure, which is used for telephone number mapping (ENUM) and could have serious privacy and security implications. It underscores the need for better oversight and security measures in critical internet infrastructure, especially when military communications are involved. The researcher did not set up a SIP server to terminate calls, but the logging of DNS queries revealed the scale of usage. The e164.arpa domain is largely non-public, with private ENUM services used for number porting, and the incident shows how such infrastructure can be accidentally compromised.

hackernews · gavide · Aug 21, 13:11 · [Discussion](https://news.ycombinator.com/item?id=49387570)

**Background**: ENUM (E.164 Number to URI Mapping) is a protocol that maps telephone numbers to Internet addresses using DNS, with the e164.arpa domain serving as the root for public ENUM. It was designed to facilitate VoIP and other IP-based telephony services, but it has seen limited public adoption and is now mostly used in private networks. The incident highlights how a misconfigured or abandoned infrastructure can become a security risk.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Telephone_number_mapping">Telephone number mapping - Wikipedia</a></li>
<li><a href="https://icannwiki.org/ENUM">ENUM - ICANNWiki</a></li>
<li><a href="https://nickvsnetworking.com/enum-dns-based-call-routing/">ENUM – DNS based Call Routing | Nick vs Networking</a></li>

</ul>
</details>

**Discussion**: The community discussion expressed amazement that the author avoided legal trouble, with some noting that reporting such issues to authorities often leads to prosecution. Others suggested the author could have gone further by setting up a SIP server to see if calls would terminate, and there was general appreciation for the story highlighting overlooked infrastructure flaws.

**Tags**: `#security`, `#DNS`, `#telephony`, `#privacy`, `#infrastructure`

---

<a id="item-4"></a>
## [Stop Making TUIs: Build Native UIs with AI Agents](https://simonwillison.net/2026/Aug/21/stop-making-tuis/) ⭐️ 7.0/10

Thomas Ptacek argues that coding agents have made building native user interfaces cheap, so developers should stop creating text-based TUIs for their tools and instead build real GUIs. Simon Willison echoes this, noting his own success with vibe-coded macOS task bar apps. This shift could significantly improve the usability of developer tools, making them more accessible to non-technical users. As AI-assisted development becomes mainstream, the barrier to creating polished UIs is lowered, potentially changing how developers approach tool design. Ptacek's post includes a practical example and a compelling quote encouraging developers to convert throwaway CLIs into native apps. Willison mentions his own vibe-coded bandwidth and GPU monitoring apps, which he uses daily, and admits he is 'running out of excuses' not to build more UIs.

rss · Simon Willison · Aug 21, 16:07

**Background**: TUI stands for Text User Interface, which are command-line-based interfaces that use text to interact with users. Vibe coding is a term coined by Andrej Karpathy, referring to using natural language prompts with LLMs to generate code. Coding agents are AI tools that can autonomously plan, write, and test code with minimal human intervention.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Vibe_coding">Vibe coding - Wikipedia</a></li>
<li><a href="https://cloud.google.com/discover/what-is-agentic-coding">What is agentic coding? How it works and use cases</a></li>
<li><a href="https://www.openhands.dev/blog/what-are-coding-agents">What Are Coding Agents? A Developer's Guide to Agentic Coding ...</a></li>

</ul>
</details>

**Tags**: `#UI/UX`, `#Developer Tools`, `#AI-assisted development`, `#Native Apps`, `#Coding Agents`

---