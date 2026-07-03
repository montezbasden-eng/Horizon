---
layout: default
title: "Horizon Summary: 2026-07-03 (EN)"
date: 2026-07-03
lang: en
---

> From 42 items, 5 important content pieces were selected

---

1. [US Bans Differential Privacy in Census Data](#item-1) ⭐️ 9.0/10
2. [llama.cpp patch runs DeepSeek V4 Flash with 1M context on RTX 5090](#item-2) ⭐️ 9.0/10
3. [crustc: Entire Rust compiler translated to C](#item-3) ⭐️ 8.0/10
4. [Understand to Participate: Avoiding Cognitive Debt with AI Agents](#item-4) ⭐️ 8.0/10
5. [Using DSPy to Optimize Datasette Agent's SQL Prompts](#item-5) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [US Bans Differential Privacy in Census Data](https://scottaaronson.blog/?p=9902) ⭐️ 9.0/10

On June 4, 2026, the U.S. Secretary of Commerce issued Directive DAO 216-26, banning noise infusion and differential privacy in all Census Bureau statistical products, restricting disclosure avoidance to coarsening only. This directive removes mathematically rigorous privacy protections from census data, potentially allowing re-identification of individuals and undermining trust in official statistics, with broad implications for research, policy, and civil rights. The ban explicitly forbids 'noise infusion' methods, including differential privacy, which were core to protecting privacy in 2020 Census data releases. Only 'coarsening'—aggregating or suppressing data—is now permitted.

hackernews · flowercalled · Jul 3, 00:01 · [Discussion](https://news.ycombinator.com/item?id=48768992)

**Background**: Differential privacy is a mathematical framework that adds controlled noise to datasets to prevent identifying individuals while preserving statistical accuracy. The Census Bureau adopted it for the 2020 Census to address privacy concerns, but critics argue it reduces data utility. The new directive reverses this approach, favoring simpler but less protective methods.

<details><summary>References</summary>
<ul>
<li><a href="https://scottaaronson.blog/?p=9902">Shtetl-Optimized » Blog Archive » An American privacy emergency...</a></li>
<li><a href="https://www.census.gov/programs-surveys/decennial-census/decade/2020/planning-management/process/disclosure-avoidance/differential-privacy.html">Understanding Differential Privacy</a></li>
<li><a href="https://www.privacyguides.org/articles/2025/09/30/differential-privacy/">What is Differential Privacy ? - Privacy Guides</a></li>

</ul>
</details>

**Discussion**: Commenters expressed confusion and concern about the political motives behind the directive, with some speculating it aims to weaken privacy protections for political gain. Others noted the lack of a clear call to action link in the original post and requested more technical details on coarsening's effectiveness.

**Tags**: `#privacy`, `#differential privacy`, `#US Census`, `#data policy`, `#surveillance`

---

<a id="item-2"></a>
## [llama.cpp patch runs DeepSeek V4 Flash with 1M context on RTX 5090](https://www.reddit.com/r/LocalLLaMA/comments/1ulymml/llamacpp_patch_deepseek_v4_flash_running_with/) ⭐️ 9.0/10

A developer patched llama.cpp with a custom CUDA kernel for the DeepSeek Lightning Indexer, enabling DeepSeek V4 Flash to run with full 1M token context on a single RTX 5090, reducing VRAM usage from ~256GB to ~31GB. This breakthrough makes state-of-the-art long-context LLMs accessible on consumer hardware, democratizing research and applications that require processing entire codebases or large documents locally. The patch implements the DSA lightning indexer as a CUDA kernel, achieving prefill speeds of 159-263 t/s and decode speeds of ~14 t/s at 1M context, with peak VRAM of ~31GB. Correctness was verified via needle-in-a-haystack tests at various depths.

reddit · r/LocalLLaMA · /u/da_dragon321 · Jul 2, 23:54

**Background**: DeepSeek V4 Flash uses a hybrid attention mechanism with Compressed Sparse Attention (CSA) and a lightning indexer to efficiently handle long contexts. The official implementation requires massive VRAM (~256GB at 1M tokens), making it impractical for consumer GPUs. llama.cpp is an open-source C/C++ LLM inference engine that enables local execution on various hardware.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/ggml-org/llama.cpp">GitHub - ggml-org/llama.cpp: LLM inference in C/C++</a></li>
<li><a href="https://github.com/antirez/llama.cpp-deepseek-v4-flash">GitHub - antirez/llama.cpp-deepseek-v4-flash: Experimental implementation of DeepSeek v4 flaash in llama.cpp · GitHub</a></li>
<li><a href="https://huggingface.co/unsloth/DeepSeek-V4-Flash">unsloth/DeepSeek-V4-Flash · Hugging Face</a></li>

</ul>
</details>

**Discussion**: The Reddit community praised the optimization, with users noting that local models like DeepSeek V4 Flash now rival API-based models in speed and quality for coding tasks. Some highlighted that while Opus and Fable still lead in quality, local models are becoming viable alternatives.

**Tags**: `#llama.cpp`, `#DeepSeek`, `#CUDA`, `#LLM`, `#optimization`

---

<a id="item-3"></a>
## [crustc: Entire Rust compiler translated to C](https://github.com/FractalFir/crustc) ⭐️ 8.0/10

A developer named FractalFir has spent three years working on crustc, a project that transpiles the entire rustc compiler (the Rust compiler) into C code, aiming to support old or obscure hardware and enable bootstrapping without LLVM. This project addresses the bootstrapping problem for Rust, allowing the compiler to be built from source without relying on LLVM, and enables Rust to run on platforms where LLVM or GCC backends are unavailable, potentially expanding Rust's reach to legacy and embedded systems. crustc is the 14th known attempt to compile Rust to C, and it leverages GCC's optimization passes after transpilation. The project is still in development and not yet complete, but it has generated significant community interest.

hackernews · Philpax · Jul 2, 22:57 · [Discussion](https://news.ycombinator.com/item?id=48768464)

**Background**: Bootstrapping is the process of building a compiler using an earlier version of itself. Rust currently requires a pre-built rustc binary or LLVM to compile, which creates a chicken-and-egg problem for new platforms. Transpiling Rust to C allows using any C compiler (like GCC) to build rustc, breaking this dependency and enabling support for architectures without LLVM.

<details><summary>References</summary>
<ul>
<li><a href="https://rustc-dev-guide.rust-lang.org/building/bootstrapping/what-bootstrapping-does.html">What Bootstrapping does - Rust Compiler Development Guide</a></li>

</ul>
</details>

**Discussion**: The community expressed admiration for the project's dedication, with one commenter noting it is the 14th attempt. A user suggested using Diverse Double-Compiling (DDC) to verify the official rustc for backdoors. Another commenter clarified that LLVM's C backend is no longer maintained, making crustc a timely alternative.

**Tags**: `#rust`, `#compiler`, `#bootstrapping`, `#transpilation`, `#c`

---

<a id="item-4"></a>
## [Understand to Participate: Avoiding Cognitive Debt with AI Agents](https://simonwillison.net/2026/Jul/2/understand-to-participate/#atom-everything) ⭐️ 8.0/10

Simon Willison highlighted Geoffrey Litt's concept of 'understand to participate' as a key principle for collaborating with AI coding agents, emphasizing the need to maintain deep understanding to avoid cognitive debt. This insight addresses a critical challenge in AI-assisted development: as agents generate large code changes, developers risk losing understanding of the codebase, leading to cognitive debt that hinders future participation and creativity. Geoffrey Litt presented this idea at the AIE conference, and his talk is available on YouTube along with a Twitter thread. The concept argues that developers must actively learn what the agent is doing to remain effective participants.

rss · Simon Willison · Jul 2, 17:07

**Background**: Cognitive debt refers to the erosion of shared understanding in a software team, making it harder to reason about and change the system. As AI coding agents become more capable, developers may accept code they don't fully understand, accumulating cognitive debt that must eventually be repaid.

<details><summary>References</summary>
<ul>
<li><a href="https://simonwillison.net/2026/Jul/2/understand-to-participate/">Understand to participate - simonwillison.net</a></li>
<li><a href="https://margaretstorey.com/blog/2026/02/09/cognitive-debt/">How Generative and Agentic AI Shift Concern from Technical Debt to Cognitive Debt</a></li>
<li><a href="https://arxiv.org/abs/2603.22106">[2603.22106] From Technical Debt to Cognitive and Intent Debt: Rethinking Software Health in the Age of AI</a></li>

</ul>
</details>

**Tags**: `#AI-assisted development`, `#cognitive debt`, `#software engineering`, `#human-AI collaboration`

---

<a id="item-5"></a>
## [Using DSPy to Optimize Datasette Agent's SQL Prompts](https://simonwillison.net/2026/Jul/2/dspy-datasette-agent-prompts/#atom-everything) ⭐️ 7.0/10

Simon Willison used the DSPy framework to automatically evaluate and improve the system prompts for Datasette Agent's SQL query generation feature, identifying issues like column-name guessing and error-retry loops. This demonstrates a practical, real-world application of DSPy for prompt optimization beyond toy examples, showing how automated evaluation can systematically improve LLM-based tools. It highlights a methodology that can be adopted by developers building AI agents that rely on structured data queries. Willison used Claude Code with Claude Fable 5 to orchestrate the experiment, and DSPy tested prompts using GPT-4.1 mini and nano. One key finding was that omitting column names in the schema listing led to guessing and error loops, suggesting either including column names or softening the advice to avoid calling describe_table.

rss · Simon Willison · Jul 2, 18:25

**Background**: DSPy is a Python framework for programming—rather than prompting—language models, allowing developers to define tasks via signatures and optimize prompts algorithmically. Datasette Agent is an AI assistant for Datasette that can execute read-only SQL queries to answer user questions. System prompt optimization is the process of automatically improving the instructions given to an LLM to enhance performance on specific tasks.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/stanfordnlp/dspy">GitHub - stanfordnlp/dspy: DSPy: The framework for ... GitHub - isaka/DSPy: DSPy: The framework for programming—not ... What Is DSPy? How It Works, Use Cases, and Resources Programming, Not Prompting: A Hands-On Guide to DSPy DSPy Framework — Programmatic Prompt Optimization (2026) Tutorials Overview - DSPy</a></li>
<li><a href="https://agent.datasette.io/">Datasette Agent: an AI assistant for Datasette to help ...</a></li>
<li><a href="https://github.com/datasette/datasette-agent">GitHub - datasette/datasette-agent: An LLM-powered agent for ...</a></li>

</ul>
</details>

**Tags**: `#DSPy`, `#prompt engineering`, `#LLM`, `#SQL`, `#Datasette`

---