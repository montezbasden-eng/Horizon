---
layout: default
title: "Horizon Summary: 2026-09-20 (EN)"
date: 2026-09-20
lang: en
---

> From 29 items, 3 important content pieces were selected

---

1. [Terry Tao: Mathematics Is More Than Proof](#item-1) ⭐️ 8.0/10
2. [PlanetScale launches Tin, a full-text search engine for Postgres](#item-2) ⭐️ 8.0/10
3. [Qwen 3.8 27B Autonomously Tackles Open Covering Design C(25,15,5) on RTX 5090](#item-3) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Terry Tao: Mathematics Is More Than Proof](https://terrytao.wordpress.com/2026/09/18/if-math-is-more-than-proof-we-need-to-better-celebrate-the-rest-of-it/) ⭐️ 8.0/10

Terry Tao published an essay arguing that mathematics encompasses far more than formal proofs—intuition, computation, exposition, and other contributions deserve greater recognition. The piece sparked a large Hacker News discussion (325 points, 248 comments) about the changing nature of mathematical work and its parallels to software engineering. The essay challenges the proof-centric reward system of academic mathematics, where tenure and prestige hinge on producing difficult proofs. As AI increasingly automates proof and computation tasks, this debate becomes urgent for mathematicians whose core work may be transformed, and it echoes broader questions about human value in an AI-driven research ecosystem. Tao's argument is not that proofs are unimportant, but that the discipline undervalues other forms of mathematical labor such as building intuition, writing exposition, developing computational tools, and verifying results. Commenters noted that computational feats like computing pi to more digits or finding new Mersenne primes count as 'math news' yet are of little interest to mathematicians, illustrating the gap between computational output and mathematical insight.

hackernews · num42 · Sep 19, 06:28 · [Discussion](https://news.ycombinator.com/item?id=49763928)

**Background**: Terry Tao is a Fields Medalist and widely regarded as one of the greatest living mathematicians. In mathematics, a proof is a rigorous logical argument establishing a theorem, and the field has traditionally treated proof production as its central activity. The philosophy of mathematical practice studies how mathematics is actually done, including the roles of intuition, explanation, and computation, which are often downplayed in formal accounts.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mathematical_proof">Mathematical proof - Wikipedia</a></li>
<li><a href="https://plato.sydney.edu.au/entries/mathematical-practice/">The Philosophy of Mathematical Practice (Stanford Encyclopedia of...)</a></li>
<li><a href="https://news.ycombinator.com/item?id=8912834">Striking parallels between mathematics and software engineering</a></li>

</ul>
</details>

**Discussion**: Commenters drew parallels to the 1900 Poincaré–Hilbert debate, arguing that Hilbert's proof-centric path marginalized intuition in modern mathematics education. Others compared mathematics to software engineering, noting that AI can automate tasks but not entire jobs—yet for many mathematicians, those tasks were the job itself, forcing a painful pivot. Some also observed that Fields Medal age limits favor raw brainpower over deep understanding, making AI's rise a natural source of anxiety.

**Tags**: `#mathematics`, `#philosophy-of-math`, `#AI-impact`, `#academia`, `#Terry-Tao`

---

<a id="item-2"></a>
## [PlanetScale launches Tin, a full-text search engine for Postgres](https://planetscale.com/blog/introducing-tin) ⭐️ 8.0/10

PlanetScale has announced Tin (short for "Text INdex"), a full-text search extension for Postgres that is now generally available (GA) for all Postgres and Neki databases. Tin adds an inverted index type built for search, BM25 relevance ranking, and a dedicated query language called TINQL. Full-text search is one of the most requested Postgres features, and Tin lets teams keep search inside their existing database instead of running a separate system like Elasticsearch. It also intensifies competition in a fast-growing field that already includes ParadeDB, pg_search, Timescale's pg_textsearch, and Neon/Databricks' Lakebase Search. Tin is only offered on PlanetScale's cloud services; the local companion extension, Lead, is mainly for testing TINQL syntax on small datasets and does not have the same performance characteristics. PlanetScale says Tin is available immediately as a GA release for all Postgres and Neki databases.

hackernews · ksec · Sep 19, 13:52 · [Discussion](https://news.ycombinator.com/item?id=49766611)

**Background**: Postgres has long shipped its own built-in full-text search based on tsvector, tsquery, and tsrank, but many users find it limited in relevance quality and index size compared with dedicated search engines. BM25 is a widely used ranking function that scores documents by term frequency and rarity, and it is the standard behind systems like Lucene and Elasticsearch. Tin packages an inverted index and BM25 ranking as a Postgres extension, so search queries can run directly against Postgres tables.

<details><summary>References</summary>
<ul>
<li><a href="https://planetscale.com/blog/introducing-tin">Introducing TIN : full-text search for Postgres — PlanetScale</a></li>
<li><a href="https://planetscale.com/docs/postgres/search">TIN : PlanetScale Postgres Search - PlanetScale</a></li>
<li><a href="https://www.postgresql.org/docs/current/textsearch.html">PostgreSQL: Documentation: 18: Chapter 12. Full Text Search</a></li>

</ul>
</details>

**Discussion**: Commenters noted that nearly every database company is now shipping full-text search, with some attributing the wave to AI-boosted coding productivity. A key concern is that Tin is cloud-only: the local Lead extension lacks the same performance, so users cannot fully test it outside PlanetScale. Others argued that Postgres' built-in full-text search is already sophisticated and questioned why they would adopt a non-core, "vibecoded" alternative.

**Tags**: `#Postgres`, `#full-text search`, `#database`, `#PlanetScale`, `#open source`

---

<a id="item-3"></a>
## [Qwen 3.8 27B Autonomously Tackles Open Covering Design C(25,15,5) on RTX 5090](https://www.reddit.com/r/LocalLLaMA/comments/1wl18ax/qwen_38_27b_running_live_on_a_rtx_5090_to_solve/) ⭐️ 8.0/10

A Reddit user launched a live experiment running Qwen 3.8 27B autonomously on an RTX 5090 to solve the open covering design problem C(25,15,5), where the current best solution uses 42 groups and the goal is 41. The experiment streams the agent's public messages, memories, life-loop, and code on a public website, with an independent checker verifying any proposed solution in real time. This experiment aims to show that open-source models, even a 27B model running on consumer hardware, can contribute to scientific discovery and innovation. It also promotes the idea that autonomous agentic research should be open and accessible to both humans and AI agents to accelerate solving important problems. The covering design problem C(25,15,5) was chosen because verifying a proposed solution is simple, making it ideal for live validation. The setup runs on an RTX 5090, a Blackwell-architecture GPU with 32 GB of GDDR7 memory and 1,792 GB/s bandwidth, and the experiment is a follow-up to a prior 63-hour autonomous run on the Riemann hypothesis.

reddit · r/LocalLLaMA · /u/GuiltyBookkeeper4849 · Sep 19, 23:41

**Background**: A (v,k,t)-covering design is a collection of k-element subsets (blocks) of {1,...,v} such that every t-element subset is contained in at least one block; the goal is to minimize the number of blocks. C(25,15,5) asks for the smallest number of 15-element blocks needed to cover all 5-element subsets of a 25-element set, and the current best known solution uses 42 blocks. Qwen 3.8 27B is a dense 27-billion-parameter vision-language model from Alibaba's Qwen lab, released under Apache 2.0, and the RTX 5090 is NVIDIA's consumer flagship GPU.

<details><summary>References</summary>
<ul>
<li><a href="https://web.archive.org/web/20120229042600/http://www.ccrwest.org:80/cover.html">La Jolla Covering Repository</a></li>
<li><a href="https://huggingface.co/Qwen/Qwen3.8-27B">Qwen/Qwen3.8-27B · Hugging Face</a></li>
<li><a href="https://www.runpod.io/articles/guides/nvidia-rtx-5090">NVIDIA RTX 5090: Specs, 32GB VRAM & AI Benchmarks (2026)</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#autonomous agents`, `#mathematical discovery`, `#covering design`, `#GPU computing`

---