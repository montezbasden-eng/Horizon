---
layout: default
title: "Horizon Summary: 2026-08-15 (EN)"
date: 2026-08-15
lang: en
---

> From 44 items, 4 important content pieces were selected

---

1. [Going Dark and the Rise of Law Enforcement Hacking](#item-1) ⭐️ 8.0/10
2. [RISC-V: A Critical Look at Architectural Choices](#item-2) ⭐️ 8.0/10
3. [Firefox Now the Last Major Browser Supporting uBlock Origin](#item-3) ⭐️ 8.0/10
4. [Don't Classify, Hallucinate: LLM Tagging via Embeddings](#item-4) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Going Dark and the Rise of Law Enforcement Hacking](https://blog.cryptographyengineering.com/2026/08/14/everything-is-about-to-go-dark/) ⭐️ 8.0/10

The article discusses the shift from traditional surveillance to law enforcement hacking as encryption limits access to communications, highlighting the 'going dark' problem and the increasing use of hacking tools by police. 这一转变对隐私、安全以及执法部门与公民之间的权力平衡具有重大影响。它影响犯罪调查的方式，并引发关于政府监控范围的合法性和伦理问题。 The article notes that law enforcement hacking relies on finding software bugs, but there may be a ceiling on the number of useful bugs. It also mentions the historical context of wiretapping, which required physical wires and was costly.

hackernews · vslira · Aug 14, 20:52 · [Discussion](https://news.ycombinator.com/item?id=49304447)

**Background**: The 'going dark' problem refers to the situation where law enforcement has legal authority to access encrypted data but lacks the technical means to do so. Encryption has become so strong that even governments cannot bypass it, leading to debates about backdoors and hacking as alternatives.

<details><summary>References</summary>
<ul>
<li><a href="https://carnegieendowment.org/research/2024/04/exploring-law-enforcement-hacking-as-a-tool-against-transnational-cyber-crime">Exploring Law Enforcement Hacking as a Tool Against ...</a></li>
<li><a href="https://observed.org/can-police-use-hacking-techniques/">Can Police Use Hacking Techniques? | Know Your Rights</a></li>
<li><a href="https://repository.law.umich.edu/mjlr/vol50/iss2/5/">"Shedding Light on the "Going Dark" Problem and the Encryption Debate" by John Mylan Traylor</a></li>

</ul>
</details>

**Discussion**: Community comments highlight the irony of the 'going dark' label given the prevalence of surveillance cameras and metadata collection. Some question the assumption that useful bugs are becoming scarce, noting that software seems to be getting buggier with AI-generated code. Others point out the historical costs and practicalities of wiretapping.

**Tags**: `#encryption`, `#law enforcement`, `#surveillance`, `#security`, `#privacy`

---

<a id="item-2"></a>
## [RISC-V: A Critical Look at Architectural Choices](https://dmitry.gr/?r=06.%20Thoughts&proj=12.%20RV) ⭐️ 8.0/10

Dmitry Grinberg published a critical analysis of RISC-V, arguing that while it is a valuable open standard, its technical design contains avoidable flaws. The article sparked a high-engagement discussion on Hacker News with 85 comments. This analysis is significant because RISC-V is rapidly gaining adoption across industries, and understanding its architectural trade-offs is crucial for developers and companies making long-term commitments. The discussion highlights the tension between technical purity and practical needs in ISA design, influencing future extensions and implementations. The article criticizes specific RISC-V design decisions, such as the base integer instruction set lacking common operations and the fragmented extension ecosystem. Commenters note that while the base ISA is simple, practical use often requires profiles like RV64GC, which add complexity.

hackernews · kaycebasques · Aug 14, 22:38 · [Discussion](https://news.ycombinator.com/item?id=49305492)

**Background**: RISC-V is a free and open standard instruction set architecture (ISA) based on RISC principles, released under permissive licenses and free to implement without royalties. Unlike proprietary ISAs like x86 and ARM, RISC-V aims to enable open collaboration and innovation in processor design. The ISA is modular, with a small base integer instruction set and optional extensions, allowing customization for different applications.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/RISC-V">RISC-V - Wikipedia</a></li>
<li><a href="https://riscv.org/">Home - RISC-V International</a></li>
<li><a href="https://docs.riscv.org/reference/isa/v20250508/_attachments/riscv-unprivileged.pdf">The RISC-V Instruction Set Manual Volume I</a></li>

</ul>
</details>

**Discussion**: The community discussion is largely supportive of the article's critique, with commenters agreeing that RISC-V's design has trade-offs. Some emphasize that the open standard aspect is more important than technical perfection, while others note that practical implementations often require extensions beyond the base ISA. A few commenters compare RISC-V to MIPS, suggesting it may face similar challenges.

**Tags**: `#RISC-V`, `#ISA`, `#CPU design`, `#open hardware`, `#architecture`

---

<a id="item-3"></a>
## [Firefox Now the Last Major Browser Supporting uBlock Origin](https://www.pcworld.com/article/3212428/firefox-is-now-the-last-major-browser-that-still-supports-ublock-origin.html) ⭐️ 8.0/10

Firefox has become the only major browser that still fully supports uBlock Origin, following Google's enforcement of Manifest V3, which restricts the webRequestBlocking API that uBlock Origin relies on. This shift marks a significant change in the browser extension landscape. This is significant because uBlock Origin is one of the most popular ad blockers, and its loss on Chrome and other Chromium-based browsers could affect millions of users who rely on it for privacy and ad blocking. Firefox's unique position may attract users seeking robust content filtering, potentially shifting browser market share. Manifest V3 removes the webRequestBlocking permission for most extensions, limiting ad blockers to the declarativeNetRequest API, which has a lower rule limit and less flexibility. An unofficial port of uBlock Origin to Manifest V3 exists on GitHub, but it faces challenges due to these restrictions.

hackernews · DemiGuru · Aug 14, 19:03 · [Discussion](https://news.ycombinator.com/item?id=49303202)

**Background**: uBlock Origin is a free, open-source browser extension for content filtering and ad blocking, developed by Raymond Hill. It has been widely used on Chrome and Firefox, with millions of active users. Google's Manifest V3, introduced to improve security and performance, restricts certain APIs, which has forced many ad blockers to adapt or become less effective.

<details><summary>References</summary>
<ul>
<li><a href="https://developer.chrome.com/docs/extensions/develop/migrate/what-is-mv3">Extensions / Manifest V3 | Chrome for Developers</a></li>
<li><a href="https://arstechnica.com/gadgets/2024/08/chromes-manifest-v3-and-its-changes-for-ad-blocking-are-coming-real-soon/">Chrome’s Manifest V3, and its changes for ad blocking, are coming real soon - Ars Technica</a></li>
<li><a href="https://en.wikipedia.org/wiki/UBlock_Origin">UBlock Origin</a></li>

</ul>
</details>

**Discussion**: Community comments express mixed sentiments: some praise Firefox for vetting uBlock Origin's code, while others criticize Google's restrictions as limiting user freedom. There is also discussion about an unofficial Manifest V3 port of uBlock Origin and questions about the effectiveness of uBlock Origin Lite.

**Tags**: `#Firefox`, `#uBlock Origin`, `#Manifest V3`, `#ad-blocking`, `#browser extensions`

---

<a id="item-4"></a>
## [Don't Classify, Hallucinate: LLM Tagging via Embeddings](https://simonwillison.net/2026/Aug/14/dont-classify-hallucinate/) ⭐️ 7.0/10

Doug Turnbull proposed a method to tag untagged content by having an LLM generate hypothetical tags without seeing the existing vocabulary, then mapping them to concrete tags using vector embeddings. Simon Willison highlighted this approach on his blog, noting its practicality for large tag corpora. This technique offers a scalable solution for tagging large corpora where the tag vocabulary is too large to feed directly to an LLM. It leverages LLM creativity and vector similarity, potentially improving information management and retrieval workflows. The method involves prompting the LLM to generate novel tags that fit the content, optionally providing examples of the tag shape. Then, vector embeddings are used to find the closest existing tags in the corpus to the hallucinated ones. This approach avoids the need to feed the entire tag list to the model.

rss · Simon Willison · Aug 14, 21:54

**Background**: LLMs can hallucinate, generating plausible but incorrect information. However, this technique turns hallucination into a feature by using it to propose candidate tags. Vector embeddings represent text as numerical vectors, allowing semantic similarity to be measured, which is key to mapping the hallucinated tags to the actual vocabulary.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2306.06085">[2306.06085] Trapping LLM Hallucinations Using Tagged Context Prompts</a></li>
<li><a href="https://qubittool.com/blog/embedding-vector-complete-guide">Vector Embeddings: Models, Search & RAG Guide (2026)</a></li>
<li><a href="https://developers.openai.com/api/docs/guides/embeddings">Vector embeddings - OpenAI API</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#tagging`, `#vector embeddings`, `#information retrieval`, `#AI`

---