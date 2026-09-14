---
layout: default
title: "Horizon Summary: 2026-09-14 (EN)"
date: 2026-09-14
lang: en
---

> From 30 items, 4 important content pieces were selected

---

1. [Fable 5.1 Solves the 370-Year-Old Cyphral Distich Cipher](#item-1) ⭐️ 8.0/10
2. [Google Still Serves Scam Ads Despite Complaints](#item-2) ⭐️ 8.0/10
3. [The Verge: Your Car Is Collecting and Selling Your Driving Data](#item-3) ⭐️ 8.0/10
4. [Perplexity Entrusts GPT-6 Astra with End-to-End Production Systems](#item-4) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Fable 5.1 Solves the 370-Year-Old Cyphral Distich Cipher](https://www.vals.ai/blogs/fable-solves-cyphral-distich) ⭐️ 8.0/10

Anthropic's Fable 5.1 AI model successfully deciphered the Cyphral Distich, a 370-year-old cryptogram consisting of two lines of 32 numbers each, found at the end of Thomas Urquhart's Logopandecteision. The result was announced in a Vals AI blog post and quickly spread across Hacker News and social media, where it drew hundreds of comments. The feat demonstrates that large language models can now tackle historical cryptanalysis problems that have resisted human researchers for centuries, potentially reshaping how historians and cryptographers approach unsolved documents. It also fuels the broader debate about whether such successes reflect genuine reasoning capability or simply the ability to exhaustively test many low-hanging hypotheses. The Cyphral Distich is a short cryptogram of two lines of 32 numbers each, embedded in a 17th-century text, and the solution was reportedly reached by feeding such unsolved cipher challenges to Fable 5.1. Fable 5.1 is Anthropic's newer model that the company says is cheaper and stronger at coding and science tasks, though for most workloads Anthropic still recommends starting with Claude Opus 5.

hackernews · u1hcw9nx · Sep 13, 21:06 · [Discussion](https://news.ycombinator.com/item?id=49688695)

**Background**: The Cyphral Distich appears at the end of Logopandecteision, a 1653 work by the Scottish writer and polymath Thomas Urquhart, and has remained unsolved for roughly 370 years. Historical ciphers like this are typically attacked by looking for patterns, known plaintext, or references in contemporary documents, a process that traditionally consumes enormous human attention. Modern LLMs offer a new approach by generating and testing many candidate interpretations at once, which is why AI-assisted cryptanalysis has become an active area of experimentation.

<details><summary>References</summary>
<ul>
<li><a href="https://www.vals.ai/blogs/fable-solves-cyphral-distich">Claude Fable 5.1 Solves the Cyphral Distich - Vals AI</a></li>
<li><a href="https://news.ycombinator.com/item?id=49688695">Fable 5.1 Solves the Cyphral Distich, a 370-year-old cipher | Hacker News</a></li>
<li><a href="https://www.anthropic.com/claude/fable">Claude Fable \ Anthropic</a></li>

</ul>
</details>

**Discussion**: Commenters were impressed but divided on significance: some noted that many such ciphers were simply never seriously attempted, suggesting these are low-hanging fruit rather than proof of deep capability, while others shared personal anecdotes of ChatGPT cracking family ciphers. A recurring theme was uncertainty about AI's trajectory, with one user describing oscillation between doom and optimism, and another joking about asking the model 'Who is Satoshi?'.

**Tags**: `#AI`, `#cryptography`, `#historical-ciphers`, `#machine-learning`, `#problem-solving`

---

<a id="item-2"></a>
## [Google Still Serves Scam Ads Despite Complaints](https://www.atomic14.com/2026/09/13/why-is-google-still-serving-dodgy-ads) ⭐️ 8.0/10

An article published on atomic14.com and a Hacker News discussion (673 points, 317 comments) examine why Google continues to serve fraudulent and scam advertisements despite widespread complaints from publishers and users. Commenters shared first-hand accounts of scam pop-ups on their sites and AI-generated scam ads on YouTube. The issue affects the entire web ecosystem, eroding user trust in online advertising and harming publishers who rely on ad networks for revenue. It also raises questions about platform accountability and whether Google's ad business incentives conflict with meaningful fraud enforcement. Publishers report that scammers rotate through free hosting domains such as azurestaticapps.net, herokuapp.com, netlify.app, and digitalocean.app, and Google reportedly refuses to let them block these domains because it treats them as TLDs. Ad fraud is estimated to have cost the industry around $44 billion in 2022, and Google's detection systems are known to miss a significant share of fraudulent activity.

hackernews · iamflimflam1 · Sep 13, 17:37 · [Discussion](https://news.ycombinator.com/item?id=49686445)

**Background**: Google Ads is the company's core advertising platform, placing ads across Google Search, YouTube, and millions of third-party websites through its AdSense network. Ad fraud refers to fraudulent activity in online advertising where automated scripts or malicious actors imitate legitimate users to generate ad revenue, and it remains a major challenge for ad networks and advertisers. The Ads Transparency Center is Google's public tool for disclosing who is advertising and what ads are running.

<details><summary>References</summary>
<ul>
<li><a href="https://www.singular.net/glossary/ad-fraud/">What is ad fraud ? | Singular</a></li>
<li><a href="https://clickguardian.ai/blog/google-ads-fraud-detection">Google Ads Fraud Detection : What Google Catches, What It Misses...</a></li>
<li><a href="https://adstransparency.google.com/?region=NL">adstransparency. google .com/?region=NL</a></li>

</ul>
</details>

**Discussion**: Commenters were largely critical of Google, with one publisher describing AdSense as a nightmare that placed thousands of scam pop-ups on their site, and another claiming Google is juicing ad revenue because AI threatens its ad business. Several called for strict liability, arguing Google is complicit, while others noted that YouTube is now full of AI-generated scam ads and that Google's review capacity is overwhelmed, relying on user reports instead.

**Tags**: `#Google Ads`, `#advertising`, `#fraud`, `#web security`, `#platform accountability`

---

<a id="item-3"></a>
## [The Verge: Your Car Is Collecting and Selling Your Driving Data](https://www.theverge.com/column/994172/your-car-is-selling-your-data) ⭐️ 8.0/10

A Verge column details how modern connected cars collect driver data—speed, location, timestamps—and sell it to third parties such as data brokers and insurers, prompting a 184-comment Hacker News discussion. Commenters shared personal experiences, technical countermeasures like Faraday cages, and noted that California's AB-1542, which would ban selling sensitive geolocation data, had passed the assembly and awaited the governor's signature. This matters because nearly every new car sold today includes embedded telematics and connectivity, meaning most drivers' behavioral data can be monetized without meaningful consent. The issue affects consumers' insurance premiums, privacy, and civil liberties, and it is driving both grassroots technical workarounds and new legislation like California's AB-1542. Commenters distinguished between two categories of data: facts about the car (VIN, spec, recall status, odometer) that outlive the owner, and facts about the driver (speed, location, timestamp) that GM sold—arguing the latter needs an outright ban rather than anonymization. Others noted that even a security-conscious owner of a seven-year-old, non-financed Volkswagen who disabled all app data collection still found mileage data reported via Carfax.

hackernews · bookofjoe · Sep 13, 13:45 · [Discussion](https://news.ycombinator.com/item?id=49683953)

**Background**: Modern cars are essentially smartphones on wheels, equipped with microphones, cameras, and telematics systems that continuously transmit data over cellular connections. Telematics—the remote measurement and transmission of vehicle data—is now standard in an estimated 91% of new US cars, and data brokers like LexisNexis Risk Solutions and Verisk aggregate this into driver behavior profiles sold to insurers. Mozilla's 2023 review of 25 car brands found every single one failed basic privacy and security standards, and the US has no comprehensive federal data protection law comparable to GDPR.

<details><summary>References</summary>
<ul>
<li><a href="https://www.ghostvault.live/blog/car-selling-driving-data">Your Car Is Selling Your Driving Data to Insurance Companies — How to Opt Out | GhostVault</a></li>
<li><a href="https://www.abc.net.au/news/science/2024-10-09/car-brands-are-tracking-and-sharing-your-data-with-third-parties/104440742">These car brands are collecting and sharing your data with third...</a></li>
<li><a href="https://www.squaredtech.co/your-car-is-spying-on-you-and-its-getting-worse">Car Data Privacy : The Shocking Truth About Your Vehicle</a></li>

</ul>
</details>

**Discussion**: The Hacker News discussion was broadly critical of the surveillance economy around cars, with users sharing personal experiences of data collection despite opt-outs and debating technical mitigations like Faraday cages. A key point of disagreement was whether the DRIVER Act adequately addresses the problem—one commenter argued it wrongly treats car facts and driver facts as the same, while others highlighted California's AB-1542 as a promising regulatory fix.

**Tags**: `#privacy`, `#automotive`, `#data-collection`, `#surveillance`, `#regulation`

---

<a id="item-4"></a>
## [Perplexity Entrusts GPT-6 Astra with End-to-End Production Systems](https://openai.com/index/perplexity-improving-accuracy-with-astra) ⭐️ 8.0/10

Perplexity is now using OpenAI's GPT-6 Astra to autonomously write communications, modify software, and monitor production systems, checking in with human oversight far less frequently than with earlier models. GPT-6 Astra was initially released to approved users on September 3, 2026, with general availability the following day. This marks a paradigm shift in how much autonomy enterprises are willing to grant AI models over critical production infrastructure, moving beyond assisted coding toward genuine end-to-end system ownership. If widely adopted, it could reshape software engineering workflows, reduce operational headcount needs, and raise new questions about accountability when autonomous agents act on live systems. The key change is the reduced frequency of human check-ins: Perplexity trusts Astra to operate with much less oversight than earlier models required, covering three distinct domains — communications, software modification, and production monitoring. The announcement comes from OpenAI's official site, underscoring the vendor's push to showcase enterprise-grade autonomous capabilities.

rss · OpenAI News · Sep 14, 00:00

**Background**: GPT-6 Astra is a large language model developed by OpenAI, succeeding earlier GPT generations with significantly enhanced autonomous reasoning and tool-use capabilities. Perplexity AI is an American company offering an AI-powered answer engine and search product. In the broader industry, AI-driven production monitoring is shifting operations from reactive to predictive by continuously analyzing machine and process data to detect anomalies early.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/GPT-6_Astra">GPT-6 Astra - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Perplexity_AI">Perplexity AI - Wikipedia</a></li>
<li><a href="https://aiquinta.ai/blog/ai-solution-for-real-time-production-monitoring-in-manufacturing/">AI solutions for real-time production monitoring in manufacturing</a></li>

</ul>
</details>

**Tags**: `#AI`, `#GPT-6`, `#Perplexity`, `#production systems`, `#automation`

---