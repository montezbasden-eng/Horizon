---
layout: default
title: "Horizon Summary: 2026-10-05 (EN)"
date: 2026-10-05
lang: en
---

> From 29 items, 3 important content pieces were selected

---

1. [Strata Runs Qwen 3.8 Flash Next 125B on RTX 4090 at 100+ Tokens/s](#item-1) ⭐️ 8.0/10
2. [Qwen3.5 9B/27B INT4 inference runs on cheap ex-mining FPGAs](#item-2) ⭐️ 8.0/10
3. [Meta's Muse agent system prompt reportedly overrides safety training with user authority](#item-3) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Strata Runs Qwen 3.8 Flash Next 125B on RTX 4090 at 100+ Tokens/s](https://github.com/Niko1221/Strata) ⭐️ 8.0/10

A GitHub project called Strata (by Niko1221) provides a one-click install for Windows and Linux that runs the 125B-parameter Qwen 3.8 Flash Next model on consumer hardware, with users reporting over 100 tokens per second on a single RTX 4090. Community members confirmed the results, with one user measuring 124 tokens/s on an RTX 4090 paired with 128GB DDR5 and a Ryzen 7950X3D. Running a 125B-parameter model at high throughput on a single consumer GPU significantly lowers the barrier to accessing frontier-class open-weight models, potentially reducing reliance on rented cloud GPUs that cost around $1 per hour. This matters for individual developers and small teams who want local, private inference without enterprise hardware. Qwen 3.8 Flash Next is a 125B-parameter MoE model with 51B additional N-gram embeddings and only 6B parameters activated per token, which is key to its efficiency. However, a community benchmark found that Strata produced a median error of 154.8 pixels on a 50-image vision coordinate task versus 46.5 pixels on llama.cpp with identical GGUF and vision adapter weights, suggesting possible quality trade-offs.

hackernews · snehesht · Oct 4, 12:51 · [Discussion](https://news.ycombinator.com/item?id=49953495)

**Background**: Qwen 3.8 Flash Next is an open-weight, 125B-parameter Mixture-of-Experts (MoE) multimodal model from Alibaba's Qwen team, built on the Qwen 4 architecture with a 262K context window. MoE models activate only a subset of parameters per token, which makes them far cheaper to run than their total size suggests. Quantization (e.g., 4-bit GGUF) compresses model weights to fit in limited GPU memory, but can degrade accuracy, especially below 4-bit.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/Niko1221/Strata">GitHub - Niko1221/Strata: Qwen3.8-Flash-Next on any consumer ...</a></li>
<li><a href="https://huggingface.co/Qwen/Qwen3.8-Flash-Next">Qwen / Qwen 3 . 8 - Flash - Next · Hugging Face</a></li>
<li><a href="https://unsloth.ai/docs/models/qwen3.8-next">Qwen 3 . 8 - Flash - Next : How to Run Locally | Unsloth Documentation</a></li>

</ul>
</details>

**Discussion**: Sentiment is largely positive, with users reporting strong real-world speeds (124 tokens/s on an RTX 4090, 255 tokens/s decode on an RTX 6000 Pro) and calling it 'game changing.' However, a11r expressed skepticism about sub-4-bit quantization degrading quality, and Jackson__ found Strata's vision accuracy notably worse than llama.cpp on the same weights, raising concerns about inference-engine fidelity.

**Tags**: `#LLM inference`, `#quantization`, `#consumer hardware`, `#Qwen`, `#performance optimization`

---

<a id="item-2"></a>
## [Qwen3.5 9B/27B INT4 inference runs on cheap ex-mining FPGAs](https://www.reddit.com/r/LocalLLaMA/comments/1wxken1/qwen35_arch_implementation_in_fpga_fabric_for/) ⭐️ 8.0/10

An enthusiast implemented Qwen3.5 9B/27B INT4 inference in custom VHDL RTL on repurposed crypto-mining FPGA cards, achieving roughly 2-3.2 tok/s generation on a $280 SQRL FK33 (8GB HBM2) at 75 MHz, with the design open-sourced under MIT on GitHub. The project also models a 27B configuration on a $375 SQRL Jungle Cat (dual XCVU35P) and projects up to ~25 tok/s with 4-way tensor parallelism at 200 MHz. It demonstrates that frontier-class 9B-27B quantized LLMs can run on scavenged, low-cost ex-mining FPGA hardware instead of scarce and expensive GPUs, offering a viable path for local inference enthusiasts. It also highlights how AI-assisted coding (Claude Opus, Kimi K3) is lowering the barrier to writing complex RTL for unconventional accelerators. On 2x FK33 at 75 MHz, prefill is ~6 tok/s for a 256-token prompt and generation drops from ~3.2 tok/s to ~2.4 tok/s at 2-3k context; output was verified layer-by-layer against llama.cpp. The Jungle Cat Lite board lacks a fast weight-loading path and GTY lane clock generation, requiring PCB rework, and the 27B model's KV cache only fits up to ~45k context on two dies (full 262k needs four dies).

reddit · r/LocalLLaMA · /u/I_am_purrfect · Oct 4, 16:51

**Background**: FPGAs are reconfigurable chips that can be programmed with custom digital logic (RTL, often written in VHDL or Verilog), unlike fixed-function GPUs. The SQRL FK33 is a Xilinx/AMD Virtex UltraScale+ XCVU33P-based mining accelerator with 8GB of HBM2 and high memory bandwidth, now nearly worthless for mining but attractive for memory-bound LLM inference. INT4 quantization shrinks model weights to 4 bits each, cutting memory footprint roughly 4x versus FP16, which is essential for fitting 9B-27B models into limited on-card memory.

<details><summary>References</summary>
<ul>
<li><a href="https://www.sqrl.stayfirst.com/forest-kitten-33/">Forest Kitten 33 | SQRL Specifications for SQRL Forest Kitten 33 | Hashrate GitHub - Zombiekilla25/fk33-fjar-miner: Open-source SHA3-256T ... Builders Are Running Qwen3.5 on FPGA Boards Scavenged From ... Developers run Qwen3.5 on repurposed crypto-mining FPGA cards ... SQRL Forest Kitten 33 | Hashrate GitHub - d953i/SQRL_FK33: SQRL FK33 board files, example ...</a></li>
<li><a href="https://github.com/Zombiekilla25/fk33-fjar-miner">GitHub - Zombiekilla25/fk33-fjar-miner: Open-source SHA3-256T ...</a></li>
<li><a href="https://mbrenndoerfer.com/writing/int4-quantization-group-wise-nf4-format-llms">INT4 Quantization: Group-wise Methods & NF4 Format for LLMs</a></li>

</ul>
</details>

**Tags**: `#FPGA`, `#LLM inference`, `#quantization`, `#local-llm`, `#hardware`

---

<a id="item-3"></a>
## [Meta's Muse agent system prompt reportedly overrides safety training with user authority](https://www.reddit.com/r/LocalLLaMA/comments/1wx8ruy/metas_muse_agent_1_in_the_app_store_system_prompt/) ⭐️ 8.0/10

A Reddit post on r/LocalLLaMA claims that the system prompt of Meta's Muse agent, which reportedly ranks #1 in the App Store, states that "the user's authority over their own household is unconditional and overrides your safety training." The claim has sparked discussion about AI safety and alignment in agentic products. If accurate, this shows a major AI company explicitly instructing an agent to let user authority override safety training, which could set a precedent for how commercial pressures erode safety guardrails in consumer AI agents. It matters for AI safety researchers, regulators, and users who rely on these agents in domestic settings. The claim is based on a reportedly leaked or shared system prompt, and the exact wording and context have not been independently verified by Meta. The phrasing specifically ties user authority to "their own household," suggesting the override is scoped to domestic tasks rather than all interactions.

reddit · r/LocalLLaMA · /u/frubberism · Oct 4, 06:37

**Background**: Muse is Meta's personal AI agent, announced on 8 September 2026, designed to carry out long-running tasks on a user's behalf rather than just answering single queries. System prompts are the hidden instructions that shape an LLM agent's behavior, and prior research has shown that commercial system prompts can override safety training, causing models to dismiss risks. This incident fits into a broader debate about how much authority AI agents should grant users, especially in sensitive contexts like the home.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Muse_(AI_agent)">Muse (AI agent) - Wikipedia</a></li>
<li><a href="https://labs.prolific.com/posts/missing-red-line">The Missing Red Line: How Commercial Pressure Erodes AI Safety ...</a></li>
<li><a href="https://www.promptingguide.ai/research/llm-agents">LLM Agents | Prompt Engineering Guide</a></li>

</ul>
</details>

**Discussion**: The Reddit thread likely contains substantive debate, with some commenters expressing alarm that a top App Store agent explicitly prioritizes user authority over safety training, while others may argue the scope is limited to household tasks and is therefore reasonable. Concerns about alignment, product design, and potential misuse are central to the discussion.

**Tags**: `#AI safety`, `#system prompts`, `#Meta`, `#LLM agents`, `#AI ethics`

---