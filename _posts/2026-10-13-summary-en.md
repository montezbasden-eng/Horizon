---
layout: default
title: "Horizon Summary: 2026-10-13 (EN)"
date: 2026-10-13
lang: en
---

> From 61 items, 4 important content pieces were selected

---

1. [AI Models Can Provably Hide Arbitrary Capabilities in Weights](#item-1) ⭐️ 8.0/10
2. [Hackers Trigger Defrosting in European Supermarket Fridges](#item-2) ⭐️ 8.0/10
3. [Developer Turns WiFi 7 Router into 320 Msps SDR Receiver](#item-3) ⭐️ 8.0/10
4. [Python 3.15 Released with PEP 810 Explicit Lazy Imports](#item-4) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [AI Models Can Provably Hide Arbitrary Capabilities in Weights](https://arxiv.org/abs/2610.13928) ⭐️ 8.0/10

A new arXiv paper (2610.13928) demonstrates that backdoor attacks can embed entire encrypted neural networks inside a host model's weights, decrypting and executing them only when a secret trigger is received. This means capability evaluations can fail to elicit hidden behaviors even when researchers have full access to the model's weights. This undermines the core assumption behind AI safety evaluations — that dangerous capabilities can always be surfaced before deployment — and raises serious concerns for open-source models, which could be distributed for free with hidden sleeper-agent backdoors. It affects model auditors, open-source AI developers, and anyone relying on capability evaluations as a security guarantee. The attack works by encrypting a neural network and embedding it within the host model's weights, so the hidden capability remains inaccessible without the secret key or trigger. The paper frames this as a provable limitation of capability elicitation under adversarial conditions, not merely an empirical observation.

hackernews · sbulaev · Oct 13, 02:07 · [Discussion](https://news.ycombinator.com/item?id=50065692)

**Background**: Capability evaluations are tests designed to surface dangerous model behaviors before deployment, and their reliability depends on the assumption that hidden capabilities can be elicited through probing or fine-tuning. A 'sleeper agent' in AI refers to a model that behaves normally until a specific trigger activates hidden malicious behavior. Backdoor attacks, which embed such triggers during training, are a known threat to open-source and third-party models.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/pdf/2610.13928">AI Models Can Provably Hide Arbitrary Capabilities - arXiv.org</a></li>
<li><a href="https://learnaivisually.com/ai-explained/digital-locker-backdoors-unelicitable-capabilities">AI Models Can Provably Hide Arbitrary Capabilities ...</a></li>
<li><a href="https://www.emergentmind.com/topics/sleeper-agents">Sleeper Agents: Covert Triggers & AI Risks - emergentmind.com</a></li>

</ul>
</details>

**Discussion**: Commenters suggested a clearer title — 'Capabilities can be hidden in AI model weights by encryption' — to avoid implying AI agents are deliberately hiding their abilities. Several expressed long-standing worry about open-source models containing sleeper-agent backdoors activated by arbitrary strings, while one commenter noted a similar effect may just be overfitting to the training environment.

**Tags**: `#AI safety`, `#model security`, `#open-source AI`, `#sleeper agents`, `#machine learning`

---

<a id="item-2"></a>
## [Hackers Trigger Defrosting in European Supermarket Fridges](https://www.tomshardware.com/tech-industry/cyber-security/unprecedented-cyberattack-cripples-supermarket-fridges-across-europe-as-hackers-activate-automatic-defrosting-delivery-and-store-prices-also-impacted-by-incident) ⭐️ 8.0/10

A cyberattack targeting internet-connected Danfoss refrigeration controllers forced automatic defrosting and raised temperatures in supermarket fridges across France and other parts of Europe, with Intermarché reporting around 150 stores affected. Attackers reportedly turned up temperatures to as high as 50°C, destroying frozen food stocks and disrupting store pricing and delivery systems. This incident shows how insecure IoT and operational technology in critical infrastructure can be weaponized to cause physical, real-world damage at scale, not just data loss. It highlights the systemic risk posed by millions of legacy, internet-exposed controllers in retail, food supply chains, and other essential services. Danfoss said the hijacked controllers were mostly legacy units running outdated firmware, and Claroty's Team82 previously disclosed multiple vulnerabilities in the Danfoss AK-SM 800A embedded web management interface. Older controllers such as the Danfoss SM800 (end of support 2021) and SC355 (end of support 2016) are suspected, and recovery options differ by device generation.

hackernews · Zeekaas · Oct 12, 12:16 · [Discussion](https://news.ycombinator.com/item?id=50055304)

**Background**: Supermarket refrigeration systems rely on supervisory controllers that coordinate compressors, defrost cycles, and temperature setpoints, and many modern units expose a web interface for remote monitoring and efficiency tuning. Danfoss is a major Danish manufacturer of such controllers, widely deployed across European retail. Because these devices often run for 15–20 years and are connected to the internet for convenience, they become attractive targets when patches are unavailable or too costly to apply.

<details><summary>References</summary>
<ul>
<li><a href="https://www.claroty.com/team82/research/freeze-the-controller-defrost-the-food-uncovering-vulnerabilities-in-danfoss-refrigeration-controllers">Freeze the Controller , Defrost the Food: Uncovering Vulnerabilities in...</a></li>
<li><a href="https://xenospectrum.com/en/france-supermarket-refrigeration-cyberattack-danfoss-legacy/">Cyberattack on Danfoss Refrigeration Controllers Hits French ...</a></li>
<li><a href="https://www.msn.com/en-us/technology/cybersecurity/danfoss-says-hacked-controllers-behind-50c-french-supermarket-fridges-ran-old-firmware/ar-AA2e6nkW">Danfoss says hacked controllers behind 50C French ... - MSN</a></li>

</ul>
</details>

**Discussion**: Commenters pointed to 15–20-year-old Danfoss controllers like the SM800 and SC355, arguing that shift-work labor and thin retail margins leave no room for security reviews or hardware refresh cycles. Others noted that newer lab and hospital equipment increasingly requires paid internet subscriptions to function, explaining why even freezers end up online, and some linked the incident to a similar August 2026 disruption at US military bases.

**Tags**: `#cybersecurity`, `#IoT`, `#critical-infrastructure`, `#legacy-systems`, `#supply-chain`

---

<a id="item-3"></a>
## [Developer Turns WiFi 7 Router into 320 Msps SDR Receiver](https://github.com/h0m3us3r/w1700k-sdr) ⭐️ 8.0/10

Developer h0m3us3r has released an open-source project that repurposes a Gemtek W1700K Wi-Fi 7 router into a wideband software-defined radio receiver, capturing raw 14-bit IQ samples at up to 320 Msps across 2.4/5/6 GHz bands. The custom firmware replaces MediaTek's firmware on the MT7996 radio and streams data over 10 GbE via zero-copy UDP to a Linux host for live spectrum and waterfall display in a browser. This hack demonstrates that consumer Wi-Fi 7 hardware can achieve high-speed SDR capabilities previously requiring expensive specialized equipment, potentially enabling budget-friendly SDR applications on everyday laptops and routers. It could significantly lower the cost barrier for RF experimentation and monitoring at 5 GHz. The receiver achieves 320 Msps, four times the 80 Msps maximum of the earlier ESP32-SDR project by the same developer, but it operates only in narrow bands, which limits its usability for many SDR use cases. The project is open-source on GitHub and leverages the Airoha AN7581 SoC for streaming.

hackernews · djfergus · Oct 12, 12:41 · [Discussion](https://news.ycombinator.com/item?id=50055593)

**Background**: Software-defined radio (SDR) is a radio communication system where components traditionally implemented in hardware are instead implemented in software, allowing flexible reception and processing of radio signals. Wi-Fi routers contain radio chipsets that can be repurposed for SDR if custom firmware is written to bypass normal Wi-Fi protocols. The MediaTek MT7996 is a Wi-Fi 7 chipset, and the Gemtek W1700K is a router that uses it.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/h0m3us3r/w1700k-sdr">Turn a WiFi 7 Router into a 320Msps Software Defined Radio ...</a></li>
<li><a href="https://www.rtl-sdr.com/turning-a-wi-fi-7-router-into-a-320-msps-sdr/">Turning a Wi-Fi 7 Router into a 320 Msps SDR - RTL-SDR</a></li>
<li><a href="https://daily.dev/posts/turn-a-wifi-7-router-into-a-320msps-software-defined-radio-receiver-38irzaw8t">Turn a WiFi 7 Router into a 320Msps Software Defined...</a></li>

</ul>
</details>

**Discussion**: Commenters are impressed by the technical achievement, with one noting it's the cheapest way to get a 320 Msps receiver at 5 GHz, while another points out the narrow-band limitation makes it unusable for most SDR use cases. Others mention that the same chipset likely works on the Banana Pi R4 and highlight the developer's earlier ESP32-SDR project.

**Tags**: `#SDR`, `#WiFi`, `#hardware hacking`, `#RF`, `#embedded systems`

---

<a id="item-4"></a>
## [Python 3.15 Released with PEP 810 Explicit Lazy Imports](https://simonwillison.net/2026/Oct/12/python-3-15/) ⭐️ 8.0/10

Python 3.15 has been released, with its What's New guide curated by release manager Hugo van Kemenade. The headline feature is PEP 810 explicit lazy imports, which let developers write `lazy import json` or `lazy from pathlib import Path` so modules load only on first use, alongside PEP 798 unpacking in comprehensions. Lazy imports directly address the startup cost that has long plagued CLI tools and plugin systems, since heavy dependencies like sentence_transformers no longer slow down every invocation. The release also marks the point where maintainers of cross-version open source software can drop Python 3.10 and begin relying on Python 3.11 features. The lazy import syntax is explicit rather than global, a deliberate contrast with PEP 690, which the Steering Council rejected in 2022 over complexity and unpredictability. PEP 798's unpacking syntax, proposed by Adam Hartz and Erik Demaine, extends the unpacking generalizations from PEP 448 that landed in Python 3.5, enabling forms like `[*sublist for sublist in lists]`.

rss · Simon Willison · Oct 12, 18:15

**Background**: Python is a widely used open source programming language, and each new release adds language features while eventually dropping support for older versions. PEPs (Python Enhancement Proposals) are the formal documents through which such changes are designed and debated before acceptance. Lazy imports defer a module's loading until its symbols are actually referenced, which can significantly reduce startup time for programs that import many heavy libraries.

<details><summary>References</summary>
<ul>
<li><a href="https://peps.python.org/pep-0810/">PEP 810 – Explicit lazy imports | peps . python .org</a></li>
<li><a href="https://socket.dev/blog/pep-810-proposes-explicit-lazy-imports-for-python-3-15">PEP 810 Proposes Explicit Lazy Imports for Python 3.15 - Soc...</a></li>
<li><a href="https://docs.python.org/3/whatsnew/3.11.html">What’s New In Python 3.11 — Python 3.15.0 documentation</a></li>

</ul>
</details>

**Tags**: `#python`, `#programming-languages`, `#release`, `#pep-810`, `#open-source`

---