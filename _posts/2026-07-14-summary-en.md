---
layout: default
title: "Horizon Summary: 2026-07-14 (EN)"
date: 2026-07-14
lang: en
---

> From 34 items, 5 important content pieces were selected

---

1. [Apple SpeechAnalyzer API Benchmarked Against Whisper](#item-1) ⭐️ 8.0/10
2. [SMP Linux Ported to Sega 32X Without Hardware Sync](#item-2) ⭐️ 8.0/10
3. [DOOMQL: A Doom-like Game Built Entirely in SQLite](#item-3) ⭐️ 8.0/10
4. [Apple M7 Ultra Chip Rumored with 1.5 TB Unified Memory](#item-4) ⭐️ 8.0/10
5. [Cache-friendly uvx usage in GitHub Actions](#item-5) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Apple SpeechAnalyzer API Benchmarked Against Whisper](https://get-inscribe.com/blog/apple-speech-api-benchmark.html) ⭐️ 8.0/10

A new benchmark compares Apple's SpeechAnalyzer API, introduced at WWDC 2025, against OpenAI's Whisper and the previous Apple speech recognition framework, showing competitive accuracy and faster on-device performance. This matters because on-device speech recognition is critical for privacy and latency-sensitive applications, and Apple's new API could reduce reliance on cloud-based services like Whisper, impacting developers and users of transcription apps. The benchmark found SpeechAnalyzer to be faster than both small and large Whisper models, with accuracy competitive to both, though each model had different quirks. SpeechAnalyzer supports streaming and speaker identification, and its size is listed as "system" with on-demand locale resources.

hackernews · get-inscribe · Jul 13, 16:06 · [Discussion](https://news.ycombinator.com/item?id=48894752)

**Background**: Whisper is an open-source speech recognition model by OpenAI, trained on 680,000 hours of data, widely used for transcription. Apple's SpeechAnalyzer, introduced at WWDC 2025, is a modular on-device speech recognition API that replaces older frameworks, offering capabilities like streaming and speaker identification.

<details><summary>References</summary>
<ul>
<li><a href="https://www.argmaxinc.com/blog/apple-and-argmax">Apple SpeechAnalyzer and Argmax WhisperKit - Argmax</a></li>
<li><a href="https://www.callstack.com/blog/on-device-speech-transcription-with-apple-speechanalyzer">On-Device Speech Transcription with Apple SpeechAnalyzer and AI SDK</a></li>
<li><a href="https://news.ycombinator.com/item?id=48894752">Apple's new SpeechAnalyzer API, benchmarked against Whisper and its predecessor | Hacker News</a></li>

</ul>
</details>

**Discussion**: Commenters noted that Whisper may not be the state-of-the-art model to benchmark against, suggesting Nvidia's Nemotron and Parakeet, Mistral's Voxtral, and Cohere Transcribe as better alternatives. Some praised SpeechAnalyzer's streaming capability and on-device processing, while others found it slightly less accurate than Whisper-Large-V2 for specific use cases like math lectures.

**Tags**: `#speech recognition`, `#Apple`, `#benchmark`, `#Whisper`, `#on-device ML`

---

<a id="item-2"></a>
## [SMP Linux Ported to Sega 32X Without Hardware Sync](https://cakehonolulu.github.io/linux-on-32x/) ⭐️ 8.0/10

Developer cakehonolulu has successfully ported SMP Linux to the Sega 32X add-on, overcoming the lack of hardware synchronization primitives by implementing Peterson's algorithm in software. This achievement demonstrates that even retro hardware without hardware synchronization support can run a modern SMP operating system, pushing the boundaries of retrocomputing and showing the versatility of Linux. The port uses Peterson's algorithm for mutual exclusion between the two SH-2 CPUs, as the 32X lacks hardware primitives like atomic instructions or cache coherency. The code is available on GitHub for further experimentation.

hackernews · cakehonolulu · Jul 13, 18:18 · [Discussion](https://news.ycombinator.com/item?id=48896600)

**Background**: The Sega 32X is a 1994 add-on for the Sega Genesis that added two Hitachi SH-2 processors for 32-bit gaming. These processors share memory but lack hardware synchronization primitives, making SMP (symmetric multiprocessing) difficult. Peterson's algorithm is a classic software-based mutual exclusion solution that uses only shared memory and works for two processes.

<details><summary>References</summary>
<ul>
<li><a href="https://cakehonolulu.github.io/linux-on-32x/">Linux on the Sega 32X. Who needs hardware synchronization primitives anyway? - cakehonolulu's blog</a></li>
<li><a href="https://en.wikipedia.org/wiki/Peterson's_algorithm">Peterson's algorithm</a></li>
<li><a href="https://en.wikipedia.org/wiki/32X">32X - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters expressed fascination with the technical feat, with some discussing hardware limitations like the SH-2's inability to write to cartridge area. Others noted the historical context of booting Linux on unconventional devices and referenced related algorithms by Lamport.

**Tags**: `#Linux`, `#retrocomputing`, `#Sega 32X`, `#SMP`, `#operating systems`

---

<a id="item-3"></a>
## [DOOMQL: A Doom-like Game Built Entirely in SQLite](https://simonwillison.net/2026/Jul/13/doomql/#atom-everything) ⭐️ 8.0/10

Developer Peter Gostev created DOOMQL, a Doom-like first-person shooter where all game logic—movement, collision, enemies, combat, and rendering—is implemented entirely in SQLite using SQL queries, including a ray tracer via recursive CTE. The game runs as a Python terminal script and was built with assistance from OpenAI's GPT-5.6 Sol model. DOOMQL demonstrates an unconventional and creative use of SQLite as a full game engine, pushing the boundaries of what a relational database can do. It inspires developers to explore novel applications of existing tools and showcases the power of modern LLMs in assisting complex coding projects. The game includes a full ray tracer implemented in a single large SQL query using recursive CTEs. The Python script creates a SQLite database that can be explored with Datasette, and the author also built a real-time HTML/JS dashboard using Datasette Apps and Claude (Fable 5) to display the game state and a minimap.

rss · Simon Willison · Jul 13, 22:34

**Background**: SQLite is a lightweight, embedded relational database engine widely used in applications. Recursive Common Table Expressions (CTEs) allow SQL queries to perform iterative operations, enabling complex computations like ray tracing. DOOMQL is a proof-of-concept that pushes SQLite beyond its typical data storage role into real-time game logic.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/GPT-5.6">GPT - 5 . 6 - Wikipedia</a></li>
<li><a href="https://openai.com/index/previewing-gpt-5-6-sol/">Previewing GPT - 5 . 6 Sol : a next-generation model | OpenAI</a></li>

</ul>
</details>

**Tags**: `#SQLite`, `#game development`, `#creative coding`, `#Python`, `#retro gaming`

---

<a id="item-4"></a>
## [Apple M7 Ultra Chip Rumored with 1.5 TB Unified Memory](https://www.reddit.com/r/LocalLLaMA/comments/1uvbzul/apple_m7_ultra_chip_planned_with_up_to_15_tb_of/) ⭐️ 8.0/10

Apple is reportedly developing the M7 Ultra chip, which could feature up to 1.5 TB of unified memory, targeting a 2028 launch. This massive unified memory capacity would enable running large-scale AI models locally on a single machine, potentially rivaling Nvidia's data-center accelerators for AI workloads. The M7 Ultra's 1.5 TB target is roughly double the capacity of the current M5 Ultra, and it is expected to use Apple's UltraFusion architecture to combine two dies.

reddit · r/LocalLLaMA · /u/Mochila-Mochila · Jul 13, 13:44

**Background**: Apple's M-series chips use unified memory, where the CPU and GPU share a single pool of high-bandwidth memory, eliminating the need to copy data between separate memory spaces. The UltraFusion interconnect, first introduced with the M1 Ultra, uses a silicon interposer to connect two dies with 2.5 TB/s bandwidth, effectively doubling performance.

<details><summary>References</summary>
<ul>
<li><a href="https://www.kucoin.com/news/flash/apple-develops-m7-ultra-chip-with-1-5tb-memory-for-ai-performance">Apple Develops M 7 Ultra Chip with 1.5TB Memory for AI... | KuCoin</a></li>
<li><a href="https://cryptobriefing.com/apple-m7-ultra-chip-ai-crypto-impact/">Apple develops M 7 Ultra chip with potential 1.5TB memory capacity...</a></li>
<li><a href="https://www.tomshardware.com/news/apple-uses-cowos-s-to-build-m1-ultra">The Tech Behind Apple's M1 UltraFusion Chip Interconnect | Tom's Hardware</a></li>

</ul>
</details>

**Tags**: `#Apple Silicon`, `#Hardware`, `#AI/ML`, `#Unified Memory`, `#LLM`

---

<a id="item-5"></a>
## [Cache-friendly uvx usage in GitHub Actions](https://simonwillison.net/2026/Jul/14/uvx-github-actions-cache/#atom-everything) ⭐️ 7.0/10

Simon Willison published a TIL post describing a cache-friendly recipe for using uvx in GitHub Actions by setting the UV_EXCLUDE_NEWER environment variable to a specific date and including that date in the cache key. This technique significantly reduces CI run times by caching tool installations, avoiding repeated downloads from PyPI on every workflow run. It is especially valuable for Python developers who frequently use uvx to run tools in GitHub Actions. The UV_EXCLUDE_NEWER variable tells uv to ignore packages published after the specified date, ensuring deterministic tool versions. By using that date in the cache key, the cache is automatically invalidated when the date is bumped, allowing tool upgrades.

rss · Simon Willison · Jul 14, 00:56

**Background**: uv is a fast Python package and project manager, and uvx is its tool for running Python-based CLI tools without installation. GitHub Actions caching can store dependencies between runs, but without careful keying, cached tools may become stale. The UV_EXCLUDE_NEWER environment variable provides a clean way to pin tool versions and control cache invalidation.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.astral.sh/uv/guides/tools/">Using tools | uv - Astral Docs</a></li>
<li><a href="https://github.com/astral-sh/uv/issues/5879">Update tests to use exclude newer environment variable · Issue #5879 · astral-sh/uv</a></li>

</ul>
</details>

**Tags**: `#GitHub Actions`, `#uv`, `#Python`, `#CI/CD`, `#caching`

---