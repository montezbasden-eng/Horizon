---
layout: default
title: "Horizon Summary: 2026-09-10 (EN)"
date: 2026-09-10
lang: en
---

> From 53 items, 6 important content pieces were selected

---

1. [OpenAI launches GPT-6 Astra, its most capable model for business](#item-1) ⭐️ 9.0/10
2. [Calif Research Unveils WeWorm, First Zero-Click WeChat Worm Built with AI](#item-2) ⭐️ 9.0/10
3. [Apple Announces iPhone Duo, Its First Foldable Phone](#item-3) ⭐️ 8.0/10
4. [Shopify acquires Tailwind Labs, maker of Tailwind CSS](#item-4) ⭐️ 8.0/10
5. [Automattic Board Forces CEO Matt Mullenweg Into Paid Leave](#item-5) ⭐️ 8.0/10
6. [IBM Releases Granite Time Series PatchTST-FM-r2 Under Commercial-Friendly License](#item-6) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [OpenAI launches GPT-6 Astra, its most capable model for business](https://openai.com/index/gpt-6-astra-next-generation-work) ⭐️ 9.0/10

OpenAI announced GPT-6 Astra, described as its most capable model for business, featuring advanced reasoning, computer use, and improved writing and design judgment. The release marks a generational leap from GPT-5.6 variants, adding enhanced multimodal capabilities across text, vision, and audio. A flagship model positioned for business with advanced reasoning and computer use could reshape enterprise AI workflows, from coding and research to autonomous agents that operate software directly. It also intensifies competition with Anthropic's Computer Use and Google's Project Jarvis in the emerging computer-using agent market. Astra runs under the model ID gpt-6-astra on OpenAI-compatible endpoints, and third-party providers such as EvoLink offer it at 10% below OpenAI list price. Community discussion highlights that its reported 'recurrent depth' or 'looped transformer' technique is essentially weight reuse across stacked layers to save GPU memory, not a fundamentally new hidden-reasoning mechanism.

rss · OpenAI News · Sep 9, 11:00

**Background**: GPT-6 Astra is OpenAI's next-generation large language model, succeeding the GPT-5.6 family and positioned as a flagship for difficult end-to-end coding, computer use, research, and agent work. 'Computer use' refers to an AI model's ability to interact with software through screenshots, mouse clicks, and keyboard input like a human, a capability pioneered by Anthropic's Computer Use and pursued by Google's Project Jarvis. 'Advanced reasoning' in modern LLMs typically means excelling at complex tasks such as puzzles, mathematical proofs, and multi-step planning, often via techniques like chain-of-thought.

<details><summary>References</summary>
<ul>
<li><a href="https://evolink.ai/blog/gpt-6-astra-api-guide">How to Use GPT - 6 Astra API: Setup, Effort & Migration</a></li>
<li><a href="https://emergent.sh/news/openai-launches-gpt-6-astra-multimodal-ai">OpenAI Launches GPT - 6 Astra : Multimodal AI Model</a></li>
<li><a href="https://www.analyticsvidhya.com/blog/2024/12/anthropic-computer-use/">Anthropic Computer Use : AI Assistant Taking Over Your Computer</a></li>

</ul>
</details>

**Discussion**: Commenters were impressed by the MSPAINT computer-use demo, calling it jaw-dropping, while others debated the technical nature of Astra's 'looped transformer' design, noting it is essentially weight reuse rather than a novel hidden-reasoning mechanism. One user reported a perceived quality regression after Tuesday, saying the model now 'feels like Sol' and expressing hope the original Astra returns.

**Tags**: `#OpenAI`, `#GPT-6`, `#LLM`, `#AI`, `#Model Release`

---

<a id="item-2"></a>
## [Calif Research Unveils WeWorm, First Zero-Click WeChat Worm Built with AI](https://simonwillison.net/2026/Sep/10/calif-research/) ⭐️ 9.0/10

Calif Research released a demo of WeWorm, described as the first zero-click worm that spreads through WeChat calls on both iOS and Android, hijacking accounts without any victim interaction. The team says it found the bug and wrote the first remote code execution (RCE) exploit in about two days with AI assistance, then built the worm in roughly one more week. This is a striking demonstration of AI's dual-use potential in offensive security: work that once required a larger team and months of effort was reportedly compressed into about a week by a small group. It raises urgent questions about how quickly AI-assisted vulnerability discovery could outpace patching and defensive capacity across widely used platforms like WeChat. The exploit succeeds even if the victim answers the call, and the victim hears nothing; exploitation takes only seconds and gives full control of the WeChat account. According to The Hacker News, Calif says Tencent has since blocked the exploit, and the release is a demo rather than a live attack tool.

rss · Simon Willison · Sep 10, 00:56

**Background**: A zero-click exploit requires no action from the victim, making it far more dangerous than attacks that need a link tap or file open. A worm is malware that self-propagates, here by using a victim's account to send malicious calls to their contacts. Remote code execution (RCE) means an attacker can run arbitrary code on the target device, in this case taking over the WeChat account on iOS and Android.

<details><summary>References</summary>
<ul>
<li><a href="https://calif.io/research/weworm">The first zero-click worm to spread through WeChat calls across iOS ...</a></li>
<li><a href="https://thehackernews.com/2026/09/wechat-zero-click-worm-took-over.html">WeChat Zero-Click Worm Took Over Accounts on iPhone and Android via Incoming Calls</a></li>
<li><a href="https://www.helpnetsecurity.com/2026/09/08/wechat-weworm-vulnerability-exploit-account-hijacking/">"Zero-click" WeChat worm could hijack accounts and spread via a single call - Help Net Security</a></li>

</ul>
</details>

**Tags**: `#ai-security-research`, `#zero-click-exploit`, `#remote-code-execution`, `#wechat`, `#ai-dual-use`

---

<a id="item-3"></a>
## [Apple Announces iPhone Duo, Its First Foldable Phone](https://www.apple.com/iphone-duo/) ⭐️ 8.0/10

Apple has officially announced the iPhone Duo, its first foldable phone, marking the company's long-awaited entry into the foldable smartphone market. The announcement sparked extensive discussion on Hacker News, generating 1,816 comments about its design, ecosystem implications, and Apple's competitive positioning. Apple's entry into the foldable phone market is a significant industry development, as it could accelerate developer adoption of foldable-optimized apps and push the entire smartphone industry toward new form factors. It also signals a strategic shift for Apple, which has historically been late to adopt hardware trends pioneered by competitors like Samsung and Chinese manufacturers. According to community hands-on impressions, the iPhone Duo's inner display reportedly has no visible crease, though some reviewers noted an inconsistency between the matte inner panel and glossy outer panel. The device is expected to encourage developers to design apps specifically for foldable form factors, addressing current issues where some Android apps either don't work or are simply stretched on foldables.

hackernews · thecosmicfrog · Sep 9, 18:15 · [Discussion](https://news.ycombinator.com/item?id=49630931)

**Background**: Foldable phones are smartphones with flexible displays that can bend in half, allowing a device to function as both a compact phone and a larger tablet. Samsung, Huawei, and other Android manufacturers have released foldable models for several years, but Apple had not entered the category until now. The iPhone Duo represents Apple's response to this growing market segment.

**Discussion**: Community sentiment was mixed: some praised the Duo's design and lack of a visible crease, while others criticized Apple for copying the Chinese smartphone playbook and noted design inconsistencies like the matte inner panel versus glossy outer panel. Android foldable owners expressed excitement that Apple's entry would push developers to properly design apps for foldables, and several commenters debated whether the device would succeed over multiple generations.

**Tags**: `#Apple`, `#foldable phones`, `#hardware`, `#mobile`, `#industry news`

---

<a id="item-4"></a>
## [Shopify acquires Tailwind Labs, maker of Tailwind CSS](https://tailwindcss.com/blog/tailwind-is-joining-shopify) ⭐️ 8.0/10

Shopify has acquired Tailwind Labs, the Canadian company behind the popular open-source utility-first CSS framework Tailwind CSS, with Tailwind's official blog announcing that the project has found a 'stable, long-term home' under Shopify while remaining MIT-licensed. The acquisition secures the future of one of the most widely used CSS frameworks in modern web development, but it also highlights how AI coding assistants are eroding the business models of open-source developer-tools companies that rely on documentation traffic and paid template sales. Tailwind Labs had reportedly laid off 75% of its engineering team in January 2026 after documentation traffic fell about 40% from early 2023 and revenue from Tailwind Plus dropped sharply; the framework itself remains free and MIT-licensed under Shopify's stewardship.

hackernews · EdwinHoksberg · Sep 9, 13:27 · [Discussion](https://news.ycombinator.com/item?id=49626190)

**Background**: Tailwind CSS is a utility-first CSS framework that lets developers style websites by composing small utility classes directly in HTML markup, rather than writing custom stylesheets. Tailwind Labs monetized the project through Tailwind Plus (formerly Tailwind UI), a paid library of prebuilt UI components and templates, with free documentation serving as the main funnel to convert users into paying customers.

<details><summary>References</summary>
<ul>
<li><a href="https://betakit.com/tailwind-finds-stable-long-term-home-with-shopify-acquisition/">Tailwind finds “stable, long-term home” with Shopify acquisition | BetaKit</a></li>
<li><a href="https://the-decoder.com/tailwinds-shattered-business-model-is-a-grim-warning-for-every-business-relying-on-site-visits-in-the-ai-era/">Tailwind's shattered business model is a grim warning for every business relying on site visits in the AI era</a></li>

</ul>
</details>

**Discussion**: Commenters largely welcomed the team's successful exit while debating AI's role: some noted that LLMs can now generate the commercial components that Tailwind sold, others questioned whether Tailwind is still needed at all when AI can write vanilla CSS, and several praised Tailwind for making them better engineers.

**Tags**: `#Tailwind CSS`, `#Shopify`, `#acquisition`, `#open-source`, `#AI impact`

---

<a id="item-5"></a>
## [Automattic Board Forces CEO Matt Mullenweg Into Paid Leave](https://techcrunch.com/2026/09/09/automattics-board-forces-ceo-matt-mullenweg-into-leave-of-absence/) ⭐️ 8.0/10

Automattic's board of directors voted to place CEO Matt Mullenweg on a paid leave of absence, a decision he announced in a company-wide Slack message and said he voted against. Mullenweg accused CFO Mark Davies of conspiring with board members Ann Dunwoody, Toni Schneider, and Sue Decker to push him out. Automattic is the company behind WordPress, which powers a large portion of the web, so a leadership shakeup there could affect millions of sites, plugins, and hosting businesses. The move also raises questions about governance and control in the WordPress open-source ecosystem, where Mullenweg has long held outsized influence. Mullenweg framed the leave as a board action taken behind his back, naming CFO Mark Davies and directors Ann Dunwoody, Toni Schneider, and Sue Decker, and noting he voted against it. The leave is paid, and it is unclear how long it will last or who will run the company day-to-day in his absence.

hackernews · LeoPanthera · Sep 9, 23:49 · [Discussion](https://news.ycombinator.com/item?id=49636283)

**Background**: Matt Mullenweg co-founded WordPress, the free and open-source content management system that runs a large share of all websites, and founded Automattic, the company that commercializes it through services like WordPress.com and WooCommerce. He has led both the WordPress project and Automattic for over two decades, giving him unusual influence over the platform's direction and ecosystem. Automattic is a fully distributed company with more than 1,700 employees across dozens of countries.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Matt_Mullenweg">Matt Mullenweg</a></li>
<li><a href="https://en.wikipedia.org/wiki/WordPress">WordPress - Wikipedia</a></li>
<li><a href="https://automattic.com/">Automattic – Making the web a better place</a></li>

</ul>
</details>

**Discussion**: Commenters largely saw the board's move as necessary but risky, with one calling it "for the best" given Mullenweg's recent "unforced error after unforced error" as CEO, while another warned that his stranglehold on Automattic and WordPress makes a major backlash likely. Others noted the oddity of the timing around his annual Burning Man trip and shared a timeline of the saga through May 2025.

**Tags**: `#Automattic`, `#WordPress`, `#leadership`, `#corporate governance`, `#open source`

---

<a id="item-6"></a>
## [IBM Releases Granite Time Series PatchTST-FM-r2 Under Commercial-Friendly License](https://huggingface.co/blog/ibm-research/ibm-releases-sota-granite-time-series) ⭐️ 7.0/10

IBM released Granite Time Series PatchTST-FM-r2 on September 9, 2026, a roughly 385-million-parameter zero-shot time-series forecasting model dual-licensed under Apache 2.0 and the Linux Foundation's OpenMDW 1.0. The model is positioned as a state-of-the-art (SOTA) time series foundation model that can be deployed in enterprise applications without restrictive licensing. The commercial-friendly dual license removes a major barrier for enterprises that want to embed time series forecasting into products and internal workflows, where restrictive or unclear licensing has often blocked adoption. It also strengthens IBM's Granite family as a credible open alternative to proprietary and research-only forecasting models. The model uses patching and channel-independent processing to handle long time series of up to 8,192 time steps, and it supports uncertainty-aware forecasting. Its 385-million-parameter scale and zero-shot design mean it can forecast without task-specific training, though users should still validate accuracy on their own domains.

rss · Hugging Face Blog · Sep 9, 15:36

**Background**: Time series foundation models are pretrained Transformer-based models that can forecast, detect anomalies, and classify patterns across many domains without building a separate model for each task. PatchTST is a well-known Transformer architecture that splits a time series into patches and processes each channel independently, which improves long-horizon forecasting. IBM's Granite family extends this line of work, and the OpenMDW 1.0 license is a permissive model license from the Linux Foundation intended to make AI models easier to use commercially.

<details><summary>References</summary>
<ul>
<li><a href="https://www.unite.ai/ibm-releases-granite-patchtst-fm-r2-zero-shot-time-series-model/">IBM Releases Granite PatchTST-FM-R2 Zero-Shot Time Series Model – Unite.AI</a></li>
<li><a href="https://github.com/ibm-granite/granite-tsfm">GitHub - ibm-granite/granite-tsfm: Foundation Models for Time Series · GitHub</a></li>
<li><a href="https://tilnote.io/en/pages/6aa192bb00d2f4a5504ae36f">Granite Time Series PatchTST-FM-r2, 성능과 상용성을 함께 고려한 시계열 모델 - TILNOTE</a></li>

</ul>
</details>

**Tags**: `#time-series`, `#foundation-models`, `#IBM`, `#open-source`, `#forecasting`

---