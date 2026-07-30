---
layout: default
title: "Horizon Summary: 2026-07-30 (EN)"
date: 2026-07-30
lang: en
---

> From 40 items, 7 important content pieces were selected

---

1. [Open-source engine runs Gemma 4 26B in 2 GB RAM on M-series Macs](#item-1) ⭐️ 9.0/10
2. [AI startups increasingly withhold research publications](#item-2) ⭐️ 8.0/10
3. [Mitchell Hashimoto Launches Superlogical, an Agentic Terminal Platform](#item-3) ⭐️ 8.0/10
4. [Two API Settings Triple GPT-5.6 ARC-AGI-3 Scores](#item-4) ⭐️ 8.0/10
5. [OpenAI Offers Free ChatGPT to 100,000 Researchers](#item-5) ⭐️ 8.0/10
6. [AI Worming through Word: Self-Replicating Prompt Injection](#item-6) ⭐️ 8.0/10
7. [Matthew Green on AI's Role in Post-Quantum Crypto Transition](#item-7) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Open-source engine runs Gemma 4 26B in 2 GB RAM on M-series Macs](https://github.com/drumih/turbo-fieldfare) ⭐️ 9.0/10

TurboFieldfare, an open-source inference engine written in Swift and Metal, can run the 4-bit quantized Gemma 4 26B-A4B-IT model on any M-series Mac using only about 2 GB of RAM by streaming experts from SSD. This technique dramatically lowers the hardware barrier for running large MoE models, enabling powerful on-device AI on consumer Macs with limited memory, and could inspire similar approaches for other models and platforms. The engine achieves 5–6 tok/s on an 8 GB M2 MacBook Air and 31–35 tok/s on an M5 MacBook Pro, using a small expert cache and bounded parallel pread to overlap SSD reads with GPU computation.

hackernews · gitpusher42 · Jul 29, 15:05 · [Discussion](https://news.ycombinator.com/item?id=49098510)

**Background**: Gemma 4 26B-A4B-IT is a Mixture-of-Experts (MoE) model from Google DeepMind with 25.2B total parameters but only 3.8B active per token. 4-bit quantization reduces its weight size to about 14 GB, which still exceeds the RAM of most Macs. Traditional inference engines require the entire model to fit in RAM, but TurboFieldfare exploits the MoE architecture by keeping only shared layers and KV cache in RAM while streaming routed experts from SSD on demand.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/collections/google/gemma-4">Gemma 4 - a google Collection</a></li>
<li><a href="https://openrouter.ai/google/gemma-4-26b-a4b-it:free">Gemma 4 26 B A 4 B (free) - API Pricing & Benchmarks | OpenRouter</a></li>
<li><a href="https://huggingface.co/blog/4bit-transformers-bitsandbytes">Making LLMs even more accessible with bitsandbytes, 4-bit ...</a></li>

</ul>
</details>

**Discussion**: The community is highly engaged, with users reporting successful runs on various M-series Macs and sharing performance benchmarks. Some users note that llama.cpp with mmap can also run large models with limited RAM, but TurboFieldfare's explicit synchronization of SSD reads with inference offers lower latency. Others appreciate the practical tips for compiling on older macOS versions.

**Tags**: `#on-device AI`, `#inference engine`, `#model quantization`, `#Mac`, `#open-source`

---

<a id="item-2"></a>
## [AI startups increasingly withhold research publications](https://www.science.org/content/article/ai-s-top-startups-are-barely-publishing-their-research) ⭐️ 8.0/10

A recent analysis reveals that top AI startups are publishing significantly less research, driven by competitive pressures and fears of intellectual property theft. The trend marks a shift from earlier open science practices in the AI community. This shift could slow the pace of AI innovation and reduce transparency, making it harder for the broader research community to build on each other's work. It also raises concerns about the privatization of knowledge in a field that has historically benefited from open collaboration. The article cites a paper that uses cumulative citations as a proxy for research significance, showing OpenAI leading, followed by companies like MEGVII, Hugging Face, and Anthropic. However, the overall trend is toward fewer publications from startups.

hackernews · YeGoblynQueenne · Jul 29, 21:25 · [Discussion](https://news.ycombinator.com/item?id=49103285)

**Background**: Historically, AI research has been characterized by open publication and sharing of code and models, accelerating progress. However, as commercial stakes rise, startups face pressure to protect proprietary advantages, leading them to limit public disclosures. This tension between open science and competitive secrecy is reshaping the AI research landscape.

**Discussion**: Commenters share personal experiences: one startup tried publishing in tier-1 journals for three years before giving up and using preprints; another avoids publishing entirely due to fear of OpenAI and Anthropic copying their work. Others criticize the 'blogification' of AI research, where unverified claims spread like social media content.

**Tags**: `#AI research`, `#startups`, `#open science`, `#publication culture`

---

<a id="item-3"></a>
## [Mitchell Hashimoto Launches Superlogical, an Agentic Terminal Platform](https://www.superlogical.com/) ⭐️ 8.0/10

Mitchell Hashimoto announced Superlogical, a new company building an agentic terminal platform on top of the open-source Ghostty terminal engine. The Ghostty project has been transferred to a non-profit organization. This marks a significant step in integrating AI agents directly into the terminal, potentially transforming how developers interact with command-line tools. By building on an open-source foundation, Superlogical could foster a new ecosystem of agentic terminal applications. Superlogical will use libghostty as a public building block, consuming the same MIT-licensed components available to everyone. The company plans to upstream shared terminal work so all libghostty consumers benefit.

hackernews · yan · Jul 29, 15:41 · [Discussion](https://news.ycombinator.com/item?id=49098965)

**Background**: Ghostty is a fast, feature-rich, cross-platform terminal emulator using platform-native UI and GPU acceleration. An 'agentic terminal' refers to a terminal that integrates AI agents to automate tasks, provide suggestions, and execute commands intelligently, similar to products like Warp.

<details><summary>References</summary>
<ul>
<li><a href="https://ghostty.org/">Ghostty</a></li>
<li><a href="https://github.com/ghostty-org/ghostty">GitHub - ghostty -org/ ghostty : Ghostty is a fast, feature-rich, and...</a></li>
<li><a href="https://www.warp.dev/">Warp — The Agentic Development Environment</a></li>

</ul>
</details>

**Discussion**: The community discussion is largely positive, with users praising the transfer of Ghostty to a non-profit and the open-source approach. Some commenters are curious about the exact product, comparing it to existing tools like tmux or agentic multiplexers, while others express skepticism about the vague description.

**Tags**: `#terminal`, `#open-source`, `#agentic`, `#Mitchell Hashimoto`, `#Ghostty`

---

<a id="item-4"></a>
## [Two API Settings Triple GPT-5.6 ARC-AGI-3 Scores](https://openai.com/index/how-two-settings-tripled-our-arc-agi-3-scores) ⭐️ 8.0/10

OpenAI reports that enabling two API settings—retained reasoning and compaction—tripled GPT-5.6's scores on the ARC-AGI-3 benchmark, improving reasoning retention and efficiency. This finding demonstrates that simple API configuration changes can dramatically improve AI reasoning performance on a challenging interactive benchmark, offering practical insights for deploying AI agents in complex environments. The two settings—retained reasoning and compaction—are already used in OpenAI's ChatGPT and Codex products. The improvement was observed on ARC-AGI-3, an interactive benchmark where agents must explore, infer goals, and plan without explicit instructions.

rss · OpenAI News · Jul 29, 15:00

**Background**: ARC-AGI-3 is an interactive benchmark that challenges AI agents to explore novel environments, acquire goals on the fly, build adaptable world models, and learn continuously without explicit instructions. It represents hundreds of original turn-based environments handcrafted by human game designers. Retained reasoning refers to preserving intermediate reasoning steps across interactions, while compaction optimizes memory usage by consolidating information.

<details><summary>References</summary>
<ul>
<li><a href="https://arcprize.org/arc-agi/3">ARC-AGI-3</a></li>
<li><a href="https://arcprize.org/blog/arc-agi-3-launch">Announcing ARC-AGI-3 - ARC Prize</a></li>

</ul>
</details>

**Tags**: `#AI`, `#benchmark`, `#GPT`, `#reasoning`, `#ARC-AGI`

---

<a id="item-5"></a>
## [OpenAI Offers Free ChatGPT to 100,000 Researchers](https://openai.com/index/chatgpt-for-academic-researchers) ⭐️ 8.0/10

OpenAI announced it will provide 100,000 academic researchers with free access to its most advanced ChatGPT models to accelerate scientific discovery. This initiative could significantly speed up research across disciplines by giving scientists powerful AI tools for data analysis, literature review, and hypothesis generation, potentially leading to breakthroughs in medicine, climate science, and more. The offer is limited to 100,000 researchers, and details on eligibility criteria, application process, and duration of access have not been fully disclosed.

rss · OpenAI News · Jul 29, 10:00

**Background**: ChatGPT is a large language model developed by OpenAI that can understand and generate human-like text. Academic researchers often face barriers in accessing cutting-edge AI tools due to cost or computational requirements. This program aims to democratize access to advanced AI for the research community.

**Tags**: `#OpenAI`, `#ChatGPT`, `#academic research`, `#AI for science`

---

<a id="item-6"></a>
## [AI Worming through Word: Self-Replicating Prompt Injection](https://simonwillison.net/2026/Jul/29/ai-worming-through-word/#atom-everything) ⭐️ 8.0/10

Security researcher Håkon Måløy discovered a novel prompt injection attack that turns Microsoft Word documents into self-replicating worms by hiding instructions that Copilot executes and propagates to new documents. This is the first demonstration of a self-replicating worm using prompt injection in an office productivity tool, highlighting a critical security vulnerability in AI-assisted workflows that could lead to widespread document infection. The attack uses hidden white-on-white text to embed instructions that Copilot interprets as user commands, causing it to manipulate the document and copy the instructions into new documents, enabling propagation without the original attacker document.

rss · Simon Willison · Jul 29, 18:43

**Background**: Prompt injection is a cybersecurity exploit where malicious inputs cause LLMs to behave unintentionally. In this variant, the attacker embeds instructions in a document that Copilot for Word later processes, treating them as legitimate user requests. The instructions then cause Copilot to replicate the hidden payload into new documents, creating a self-replicating worm.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Prompt_injection_attack">Prompt injection attack</a></li>
<li><a href="https://en.wikipedia.org/wiki/Self-replicating_computer_program">Self-replicating computer program</a></li>

</ul>
</details>

**Discussion**: The Hacker News discussion highlights the novelty of self-replication in prompt injection attacks and notes that Microsoft has not yet provided a comprehensive fix after 144 days of disclosure.

**Tags**: `#prompt injection`, `#AI security`, `#Microsoft Copilot`, `#self-replicating worm`, `#LLM vulnerabilities`

---

<a id="item-7"></a>
## [Matthew Green on AI's Role in Post-Quantum Crypto Transition](https://simonwillison.net/2026/Jul/29/matthew-green/#atom-everything) ⭐️ 8.0/10

Matthew Green highlights that the current transition to post-quantum cryptography is an ideal time for AI-driven cryptanalysis to strengthen confidence in new algorithms, referencing Anthropic's recent work and the HAWK standard. This insight from a respected cryptographer underscores the critical timing of the post-quantum transition and the potential for AI to either validate or undermine new cryptographic standards, affecting global security infrastructure. Green references Impagliazzo's Minicrypt world as a scenario where AI could undermine all hard problems, but notes that in the best case, AI cryptanalysis would make the literature more robust and increase confidence in post-quantum algorithms like HAWK.

rss · Simon Willison · Jul 29, 18:18

**Background**: Post-quantum cryptography (PQC) aims to develop algorithms secure against quantum computers. The HAWK standard is based on the Lattice Isomorphism Problem, believed hard for quantum attacks. Impagliazzo's Five Worlds classify possible computational complexity realities, with Minicrypt being one where one-way functions exist but public-key cryptography is impossible.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Post-quantum_cryptography">Post - quantum cryptography - Wikipedia</a></li>
<li><a href="https://blog.computationalcomplexity.org/2004/06/impagliazzos-five-worlds.html">Computational Complexity: Impagliazzo's Five Worlds</a></li>
<li><a href="https://thecybersecguru.com/future-sec/claude-mythos-hawk-aes-cryptanalysis/">Claude AI Discovers New Attacks Against Post - Quantum ...</a></li>

</ul>
</details>

**Tags**: `#cryptography`, `#post-quantum`, `#AI`, `#cryptanalysis`, `#standards`

---