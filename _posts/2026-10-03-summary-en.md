---
layout: default
title: "Horizon Summary: 2026-10-03 (EN)"
date: 2026-10-03
lang: en
---

> From 49 items, 5 important content pieces were selected

---

1. [AI Ataraxos Beats Best Stratego Player, Solving Imperfect-Information Game](#item-1) ⭐️ 8.0/10
2. [Redis creator antirez launches ds4, a local LLM inference engine](#item-2) ⭐️ 8.0/10
3. [OpenAI Publishes Practical Guide for Building with GPT-6 Family](#item-3) ⭐️ 8.0/10
4. [iPhone as Second GPU Speeds Up MacBook LLM Prefill by 29-44%](#item-4) ⭐️ 8.0/10
5. [AllenAI open-sources AstaBrief 8B for fast scientific report generation](#item-5) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [AI Ataraxos Beats Best Stratego Player, Solving Imperfect-Information Game](https://arstechnica.com/science/2026/10/ai-finally-beat-the-best-stratego-player-in-history-and-did-it-on-a-budget/) ⭐️ 8.0/10

A team from Carnegie Mellon, MIT, NYU, and Stanford built an AI called Ataraxos that beat Pim Niemeijer, arguably the best Stratego player ever, 15 games to one with four draws. It trained using only 16 GPUs and a few thousand dollars, playing roughly 34 times fewer games than DeepMind's DeepNash. Stratego had long stumped AI because players cannot see each other's pieces, making it a hard imperfect-information game. Solving it with a highly sample-efficient algorithm shows AI can handle hidden-information decision-making at far lower cost, with implications for real-world planning under uncertainty. The work is backed by a Nature paper and an arXiv preprint (2511.07312), and the algorithm's sample efficiency is the key breakthrough: it learned far faster than DeepNash while ending up much stronger. The main caveat is that hidden information makes optimal moves fundamentally unknowable, so the agent must reason under uncertainty rather than search exact lines.

hackernews · PaulHoule · Oct 2, 14:11 · [Discussion](https://news.ycombinator.com/item?id=49933740)

**Background**: Stratego is a chess-like two-player board game on a 10x10 grid where each side controls 40 ranked pieces with Napoleonic insignia, and the goal is to capture the opponent's Flag or all movable pieces. Unlike chess, where all pieces are visible, Stratego hides piece identities from the opponent, making it an imperfect-information game. In such games, the best move depends on information a player does not have, so standard lookahead search ('if I do this, they will do that') breaks down. DeepMind's DeepNash was a 2022 milestone that mastered Stratego but required enormous compute.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Stratego">Stratego - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Perfect_information">Perfect information - Wikipedia</a></li>
<li><a href="https://arxiv.org/abs/2401.14226">[2401.14226] Sample Efficient Reinforcement Learning by ...</a></li>

</ul>
</details>

**Discussion**: Commenters highlighted sample efficiency as the critical piece, noting that in hidden-information games a move's quality depends on unknowable information, which makes lookahead search impossible. Others shared nostalgic Stratego memories, including one who discovered a friend had subtly marked pieces to cheat, and one lamented that they had planned to build the first winning bot themselves.

**Tags**: `#AI`, `#game-playing`, `#imperfect-information`, `#reinforcement-learning`, `#research-breakthrough`

---

<a id="item-2"></a>
## [Redis creator antirez launches ds4, a local LLM inference engine](https://dwarfstar.sh/) ⭐️ 8.0/10

Salvatore Sanfilippo (antirez), the creator of Redis, has released ds4 (DwarfStar 4), a specialized local inference engine written in C for running large language models such as DeepSeek V4 Flash on personal hardware. The project quickly gained over 7,000 GitHub stars within days of release and supports Metal on macOS and CUDA on Linux. This matters because a highly respected systems programmer is bringing his minimalist, performance-focused approach to the fast-growing local LLM space, offering an alternative to heavier engines like Ollama, LM Studio, and llama.cpp. It signals that running capable models locally on consumer hardware is becoming practical and attracting serious engineering talent. ds4 is written in pure C and is model-specific, currently optimized for DeepSeek V4 Flash, with community members adding support for Vision and Qwen models. It runs on Apple Silicon Macs via Metal and on Linux via CUDA, and an active ecosystem of forks, FFI bindings, and Go bindings (ds4go) is already forming around it.

hackernews · fibo · Oct 2, 18:01 · [Discussion](https://news.ycombinator.com/item?id=49936575)

**Background**: An inference engine is the software that actually runs a trained large language model, handling tasks like loading weights, managing memory, and generating text. Most engines such as llama.cpp or Ollama aim to support many models generically, while ds4 takes a model-specific approach, tailoring the code to one architecture for maximum efficiency. Salvatore Sanfilippo, known as antirez, created Redis, a widely used in-memory database, and has recently been building minimalist pure-C implementations of AI models.

<details><summary>References</summary>
<ul>
<li><a href="https://www.youtube.com/watch?v=7_pXlTiJ240">ds 4 : antirez's New Inference Engine — 7.1k Stars in 4 Days - YouTube</a></li>
<li><a href="https://abit.ee/en/artificial-intelligence/redis-voxtral-speech-recognition-c-mistral-antirez-machine-learning-ai-en">Redis Creator Built Speech Recognition in Pure C Without Python and...</a></li>

</ul>
</details>

**Discussion**: The Hacker News discussion is substantive and largely positive: one contributor maintains a fork of ds4 as shared libraries for FFI use and built ds4go with tools for workspace editing and persistence, while another user reports running it daily on an M5 Max with 128GB and calls it the best launcher they've used. Others share inspired projects like a small Intel Xe-LP inference engine (xenolith) and ask deeper questions about what domain expertise is needed to write model-specific engines.

**Tags**: `#LLM`, `#local-inference`, `#Redis`, `#AI`, `#open-source`

---

<a id="item-3"></a>
## [OpenAI Publishes Practical Guide for Building with GPT-6 Family](https://openai.com/index/practical-guide-building-gpt-6) ⭐️ 8.0/10

OpenAI published a practical guide for startups on selecting and deploying GPT-6 models, covering reasoning effort tuning, prompt and skill improvement, tool coordination, and preparing workflows for production. The guide highlights that the GPT-6 family can now take on tasks spanning hours or days. As a major model family from OpenAI, GPT-6 adoption will shape how startups and developers architect AI products, and an official deployment guide lowers the barrier to production use. It signals that the ecosystem is shifting from single-prompt interactions toward long-horizon, tool-coordinated agentic workflows. The GPT-6 family includes multiple tiers such as GPT-6 Astra, the highest-capability model for demanding reasoning, coding, and research, alongside GPT-6 Sol and GPT-6 Luna. The guide emphasizes tuning reasoning effort and coordinating tools, reflecting that reasoning quality can still degrade on multi-path problems without careful configuration.

rss · OpenAI News · Oct 2, 16:15

**Background**: GPT-6 is OpenAI's latest family of large language models, succeeding earlier generations and designed for complex, multi-step work. Reasoning tuning refers to adjusting how much internal computation a model spends on a problem, while tool coordination means letting an AI agent connect to multiple applications and move information between them automatically. These capabilities matter because agentic workflows increasingly require models to plan, call tools, and maintain consistency over long tasks.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/practical-guide-building-gpt-6/">A model guide for the GPT - 6 family | OpenAI</a></li>
<li><a href="https://kie.ai/gpt-6-1-sol">GPT 6 .1 Sol API – Near GPT - 6 Astra Performance at Lower Cost | Kie AI</a></li>
<li><a href="https://www.linkedin.com/posts/gtayyem_chatgpt-gpt6-artificialintelligence-activity-7508290475984859136-4O1I">OpenAI Expands GPT - 6 Family with Sol and Luna Models | LinkedIn</a></li>

</ul>
</details>

**Tags**: `#GPT-6`, `#OpenAI`, `#LLM deployment`, `#prompt engineering`, `#AI startups`

---

<a id="item-4"></a>
## [iPhone as Second GPU Speeds Up MacBook LLM Prefill by 29-44%](https://www.reddit.com/r/LocalLLaMA/comments/1wvz1ex/i_made_my_iphone_a_second_gpu_for_my_24_gb/) ⭐️ 8.0/10

A developer created a fork of llama.cpp that offloads the later layers (41-64) of Qwen 3.8 27B to an iPhone 17 Pro Max's GPU over a 10 Gb/s USB-C cable, achieving 29-44% faster prefill on a 24 GB M4 Pro MacBook. The setup also extends usable context by storing up to 5.7 GB of KV cache on the phone, allowing the Mac to handle 128k context at 8-bit. This hack demonstrates a creative way to overcome unified memory limits on Apple Silicon Macs by leveraging idle iPhone hardware, potentially enabling larger models and longer contexts for local LLM enthusiasts. It highlights the growing trend of distributed inference across consumer devices and the untapped potential of mobile GPUs and Neural Engines for AI workloads. The phone runs layers 41-64 using Metal 4 tensor ops on the A19 Pro GPU, which are 2.4x faster than without them. Past 64k context, the phone switches to holding old KV pages and computing attention over old keys, with the Neural Engine compiling 16k-key pages into models; at 140k this reduced writing time from 279 to 176 ms per token. The fork also includes SME2 kernels and DFlash2 speculative decoding, boosting generation from 11.3 tok/s (stock) to 25 tok/s at ~30k context.

reddit · r/LocalLLaMA · /u/StayLameBro · Oct 2, 16:59

**Background**: Local LLM inference on Apple Silicon Macs is constrained by unified memory, which is shared between CPU and GPU; a 24 GB MacBook can only fit a 27B model at 4-bit quantization with limited context. Qwen 3.8 27B is a dense vision-language model, and IQ4_XS is a 4.25-bit non-linear quantization format that reduces model size while preserving quality. Metal 4 introduces tensor operations that leverage neural accelerators on newer Apple chips, enabling efficient matrix multiplication on the GPU.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/Qwen/Qwen3.8-27B">Qwen/Qwen3.8-27B · Hugging Face</a></li>
<li><a href="https://www.local-llm.net/learn/quantization-explained/">Understanding LLM Quantization : GGUF, GPTQ, AWQ... | local-llm.net</a></li>
<li><a href="https://developer.apple.com/metal/whats-new/">What’s New - Metal - Apple Developer</a></li>

</ul>
</details>

**Tags**: `#local-llm`, `#distributed-inference`, `#apple-silicon`, `#metal`, `#quantization`

---

<a id="item-5"></a>
## [AllenAI open-sources AstaBrief 8B for fast scientific report generation](https://huggingface.co/blog/allenai/astabrief) ⭐️ 7.0/10

AllenAI (Ai2) has open-sourced AstaBrief 8B, an open-weights model that turns a research question and retrieved literature excerpts into a cited scientific report. It is now available as the Fast mode in Asta's "Generate a report" feature, alongside the existing Claude-powered Thinking mode, and the model and its training data have been released for others to study, reproduce, and build upon. This release shows that a small, purpose-built open model can match or approach the performance of much larger proprietary models for a specialized scientific task, giving researchers and institutions a way to run report generation on their own hardware, even behind a firewall, without relying on a proprietary API. It also adds a practical, reproducible tool to the growing ecosystem of open scientific AI agents. AstaBrief is an 8B-parameter open-weights model, and Ai2's stated goal was to test whether a small model trained specifically for scientific report generation could match larger general-purpose models. Because the weights are open, institutions can deploy it on their own infrastructure, and the accompanying training data release supports reproduction and further research.

rss · Hugging Face Blog · Oct 2, 15:19

**Background**: Asta is Ai2's scholarly research assistant that draws on more than 108 million abstracts and 12 million full-text papers to find, summarize, and analyze scientific evidence. It combines literature understanding with data-driven discovery and agentic tools for researchers. AstaBrief is the first production use of a report-generation model inside Asta, providing an open-weights Fast mode next to the existing Thinking mode.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/blog/allenai/astabrief">Open-sourcing AstaBrief, the fast report-generation model in Asta</a></li>
<li><a href="https://allenai.org/blog/astabrief">Open-sourcing AstaBrief, the fast report-generation model in Asta</a></li>
<li><a href="https://www.unite.ai/ai2-open-sources-astabrief-8b-for-fast-scientific-report-generation/">Ai2 Open-Sources AstaBrief 8B for Fast Scientific Report ...</a></li>

</ul>
</details>

**Tags**: `#open-source`, `#report-generation`, `#NLP`, `#AI`, `#Hugging Face`

---