---
layout: default
title: "Horizon Summary: 2026-10-11 (EN)"
date: 2026-10-11
lang: en
---

> From 30 items, 3 important content pieces were selected

---

1. [Nvidia Reportedly Halts RTX 5090 Production to Prioritize AI GPUs](#item-1) ⭐️ 8.0/10
2. [Custom CUDA megakernel hits 140 tok/s for Qwen3.8-27B on a single RTX 3090](#item-2) ⭐️ 8.0/10
3. [WallHop Emerges as Replacement for Defunct 12ft.io Paywall Bypass](#item-3) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Nvidia Reportedly Halts RTX 5090 Production to Prioritize AI GPUs](https://www.reddit.com/r/LocalLLaMA/comments/1x2hs1e/no_more_rtx_5090/) ⭐️ 8.0/10

Nvidia has reportedly stopped producing the GeForce RTX 5090, redirecting its GB202 chips toward AI data center and professional RTX Pro GPUs instead. An RTX 5080 24GB model is rumored to become the new gaming flagship, replacing the current 16GB version. This signals a major shift in Nvidia's priorities toward AI infrastructure over consumer gaming, potentially causing a supply drought and higher prices for the RTX 5090. Local LLM enthusiasts who rely on the 5090's 32GB of VRAM for model inference will be directly affected, as they may need to seek alternative hardware or pay inflated prices. The RTX 5090 is based on the Blackwell architecture with 32GB of GDDR7 VRAM and a 575W TDP, making it highly sought after for local LLM workloads. The rumored RTX 5080 24GB would offer less VRAM than the 5090, which could limit the size of models that can be run locally.

reddit · r/LocalLLaMA · /u/Hot_Arachnid3547 · Oct 10, 15:16

**Background**: The GeForce RTX 50 series was announced at CES 2025 and launched in January 2025, based on Nvidia's Blackwell architecture with fourth-generation RT cores and fifth-generation Tensor Cores. The RTX 5090 is the flagship consumer GPU, featuring 32GB of GDDR7 memory, while the RTX 5080 uses the GB203 GPU with 16GB. Nvidia has increasingly prioritized AI data center products due to surging demand for AI compute.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/RTX_5090">RTX 5090</a></li>
<li><a href="https://www.eteknix.com/rtx-5090-discontinued-gb202-rtx-pro-rumour/">RTX 5090 Discontinued? NVIDIA Reportedly Moves GB202... - eTeknix</a></li>
<li><a href="https://wccftech.com/nvidia-axes-rtx-5090-production-gamers-get-rtx-5080-24-gb/">NVIDIA Reportedly Axes RTX 5090 Production, Diverting GB202 Chips...</a></li>

</ul>
</details>

**Tags**: `#nvidia`, `#gpu`, `#local-llm`, `#hardware`, `#ai-infrastructure`

---

<a id="item-2"></a>
## [Custom CUDA megakernel hits 140 tok/s for Qwen3.8-27B on a single RTX 3090](https://www.reddit.com/r/LocalLLaMA/comments/1x2erdj/qwen3827b_on_a_single_3090_140_toks_on_code_with/) ⭐️ 8.0/10

A developer used Claude Opus 5.5 to write a custom CUDA megakernel for Qwen3.8-27B on an RTX 3090, achieving 140 tok/s on code generation versus 73 tok/s for llama.cpp with MTP, a 1.9x speedup. The kernel runs each entire speculative-decoding cycle in a single launch, so verifying 4-5 drafted tokens costs roughly the same as verifying one. This shows that large, hand-tuned kernel fusion can deliver substantial speedups over mature general-purpose inference engines like llama.cpp on consumer hardware, making local 27B-class models far more usable for interactive coding. It also demonstrates that AI-assisted code generation can produce non-trivial low-level CUDA optimizations that were previously the domain of specialized systems teams. The megakernel is an OpenAI-compatible server that acts as a drop-in replacement for the llama server, with prefill around 1,600 tok/s versus 1,100 tok/s and 95 tok/s versus 56 tok/s when a 4K-token file is in context. Caveats: it is built specifically for unsloth's Q4_K_M quantization on 3090s only, outputs match llama.cpp except for rare rounding near-ties, and the KVCache is fp16 up to roughly 80k context before switching to q8.

reddit · r/LocalLLaMA · /u/Adorable_Weakness_39 · Oct 10, 13:01

**Background**: Speculative decoding is an inference-time optimization in which a small draft model proposes several candidate tokens and the larger target model verifies them in a single forward pass, generating multiple tokens per step instead of one. A megakernel fuses an entire decoding step into one CUDA kernel launch, avoiding the overhead of many small kernel launches that conventional engines like vLLM, TensorRT-LLM, and SGLang incur. Q4_K_M is a widely used 4-bit quantization format in llama.cpp that shrinks model weights enough to fit large models on consumer GPUs.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Speculative_decoding">Speculative decoding - Wikipedia</a></li>
<li><a href="https://theorempath.com/topics/megakernels">Megakernels . End-to-End Fused LLM Inference ... | TheoremPath</a></li>
<li><a href="https://github.com/ggml-org/llama.cpp/blob/master/tools/quantize/README.md">llama.cpp/tools/quantize/README.md at master · ggml-org/llama.cpp</a></li>

</ul>
</details>

**Tags**: `#LLM inference`, `#CUDA`, `#speculative decoding`, `#local LLM`, `#performance optimization`

---

<a id="item-3"></a>
## [WallHop Emerges as Replacement for Defunct 12ft.io Paywall Bypass](https://wallhop.io/) ⭐️ 7.0/10

A developer launched WallHop, a new paywall bypass tool, after the popular 12ft.io service shut down. The tool reportedly works on major paywalled sites like WSJ, FT, and NYT, and has drawn significant attention on Hacker News with 195 points and 85 comments. WallHop fills a gap left by 12ft.io's shutdown, giving users a way to access paywalled news without subscriptions. Its arrival reignites debates over the ethics, legality, and long-term sustainability of paywall bypass tools in the open-source community. WallHop reportedly avoids the reCAPTCHA challenges that plague archive.today, making it more convenient for some users, though it failed on at least one site (The Hindu). The developer modified a GPL-3 licensed tool called Ladder, raising questions about whether the source code should be released.

hackernews · TheWaffleHax · Oct 11, 00:46 · [Discussion](https://news.ycombinator.com/item?id=50038634)

**Background**: 12ft.io was a website created by Thomas Millar that allowed users to bypass some online paywalls by disabling JavaScript, but it was shut down. Paywall bypass tools like WallHop, RemovePaywall, and Bypass Paywalls aim to let readers access articles without paying or logging in, often by exploiting weak paywall implementations. These tools operate in a legal gray area and frequently face takedowns, prompting debates about open-source licensing and sustainability.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/12ft">12 ft - Wikipedia</a></li>
<li><a href="https://alternativeto.net/software/bypass-paywalls/">Bypass Paywalls Alternatives: Top 9 Paywall ... | AlternativeTo</a></li>
<li><a href="https://www.removepaywall.com/">RemovePaywall | Free online paywall remover</a></li>

</ul>
</details>

**Discussion**: Commenters are divided: some argue WallHop should be open source, especially since it modified a GPL-3 tool, while others believe such tools should never be open source to avoid takedowns. Others suggest alternative models like tip jars or ad-supported access, and some note WallHop's convenience over archive.today but question its longevity.

**Tags**: `#paywall bypass`, `#open source`, `#web tools`, `#ethics`, `#sustainability`

---