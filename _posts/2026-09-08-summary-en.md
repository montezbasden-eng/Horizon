---
layout: default
title: "Horizon Summary: 2026-09-08 (EN)"
date: 2026-09-08
lang: en
---

> From 39 items, 5 important content pieces were selected

---

1. [Factoring 512-bit RSA Keys of a 1990s CA on a Consumer GPU](#item-1) ⭐️ 8.0/10
2. [TALA Layout Engine for D2 Diagrams Now Open Source](#item-2) ⭐️ 8.0/10
3. [Broadcom Pulls VDDK Downloads, Complicating VMware Migration](#item-3) ⭐️ 8.0/10
4. [Abusive AI Crawlers Burn 14 CPU Cores on git.kernel.org](#item-4) ⭐️ 7.0/10
5. [OpenAI Chief Scientist Advocates for Defensive AI, Warns Against Reckless Racing](#item-5) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Factoring 512-bit RSA Keys of a 1990s CA on a Consumer GPU](https://mcpherrin.ca/2026/09/07/rsa.html) ⭐️ 8.0/10

The author successfully factored the RSA keys of a Certificate Authority from the 1990s using a consumer GPU, taking about two days. This demonstrates that 512-bit RSA keys, once considered secure, are now easily breakable with modern hardware. This highlights the vulnerability of historical encrypted communications and raises concerns about retroactive decryption by governments or other actors who may have recorded traffic. It underscores the importance of using sufficiently long key lengths in modern cryptography. The factoring was performed on a consumer GPU, taking approximately two days. The author also created a custom TLS implementation to interact with the old CA, as modern libraries like Go's crypto/tls have dropped support for SSLv3 and other legacy protocols.

hackernews · ahlCVA · Sep 8, 01:16 · [Discussion](https://news.ycombinator.com/item?id=49604637)

**Background**: RSA is a widely used public-key cryptosystem where security relies on the difficulty of factoring large composite numbers. In the 1990s, 512-bit RSA keys were common, but by 1999, RSA-155 (512 bits) was factored using the Number Field Sieve method. Modern GPUs and improved algorithms have made such factoring much faster, and 512-bit keys are now considered trivially breakable.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/RSA_numbers">RSA numbers - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/RSA_Factoring_Challenge">RSA Factoring Challenge - Wikipedia</a></li>
<li><a href="https://www.iacr.org/archive/eurocrypt2000/1807/18070001-new.pdf">Factorization of a 512–bit RSA Modulus ⋆</a></li>

</ul>
</details>

**Discussion**: Commenters expressed mixed reactions: some appreciated the technical demonstration but criticized the reliance on AI for explanations, while others raised questions about the factoring methodology and the implications for retroactive decryption. There was also interest in the custom TLS implementation for hyper-compatible websites.

**Tags**: `#RSA`, `#cryptography`, `#security`, `#historical`, `#GPU`

---

<a id="item-2"></a>
## [TALA Layout Engine for D2 Diagrams Now Open Source](https://d2lang.com/blog/tala-is-open-source/) ⭐️ 8.0/10

TALA, the proprietary layout engine developed by Terrastruct for D2 diagrams, has been open-sourced. The announcement was made on the D2 blog, making the engine freely available to the community. This move is significant for the diagramming community as it provides a high-quality automatic layout option for architecture diagrams, potentially improving tooling and workflows. It may also encourage broader adoption of D2 by removing the cost barrier for individual developers. TALA is a separate install from D2, and users can specify it via the environment variable D2_LAYOUT. The engine is designed specifically for software architecture diagrams and powers all diagrams on D2 Studio.

hackernews · alixanderwang · Sep 7, 23:37 · [Discussion](https://news.ycombinator.com/item?id=49604150)

**Background**: D2 is a modern diagram scripting language that turns text into diagrams, similar to Graphviz or Mermaid. TALA was previously a proprietary layout engine that aimed to improve automatic layout for complex diagrams, especially architecture diagrams, which often suffer from poor default layouts.

<details><summary>References</summary>
<ul>
<li><a href="https://d2lang.com/tour/tala/">TALA | D2 Documentation</a></li>
<li><a href="https://terrastruct.com/tala/">TALA | Terrastruct's AutoLayout Approach</a></li>
<li><a href="https://github.com/terrastruct/TALA">GitHub - terrastruct/TALA: A diagram layout engine designed specifically for software architecture diagrams · GitHub</a></li>

</ul>
</details>

**Discussion**: Community reactions are generally positive, with users expressing happiness about the open-sourcing and noting that TALA often provides significant improvements over default and ELK layouts. However, some users point out that TALA's output can be worse for certain graph types, such as the Go queue example, where it disrupts logical grouping and flow.

**Tags**: `#open-source`, `#diagramming`, `#layout-engine`, `#D2`, `#developer-tools`

---

<a id="item-3"></a>
## [Broadcom Pulls VDDK Downloads, Complicating VMware Migration](https://www.virtualizationhowto.com/2026/09/leaving-vmware-just-got-harder-after-broadcom-pulled-vddk-downloads/) ⭐️ 8.0/10

Broadcom has removed public downloads of the VMware Virtual Disk Development Kit (VDDK) without prior announcement, breaking migration tools that rely on it. Red Hat, a key partner, confirms it cannot redistribute the proprietary package and is exploring alternatives. This move significantly increases the difficulty and cost for VMware users to migrate to other hypervisors, effectively locking them into the platform. It signals Broadcom's strategy to extract maximum value from VMware's declining user base, affecting enterprises, cloud providers, and the broader virtualization ecosystem. VDDK is a proprietary library that allows third-party software to read VMware virtual disks from outside the hypervisor, essential for backup and migration tools. The removal affects tools like Red Hat's migration solution and Apache CloudStack, which rely on VDDK for cross-platform VM conversion.

hackernews · josephcsible · Sep 7, 20:32 · [Discussion](https://news.ycombinator.com/item?id=49602699)

**Background**: VDDK provides APIs for managing virtual disks and snapshots, enabling backup and migration software to interact with VMware ESXi hosts. Broadcom acquired VMware in 2023 and has since made controversial changes, including subscription-only licensing and layoffs, leading many users to consider alternatives like Proxmox or Hyper-V.

<details><summary>References</summary>
<ul>
<li><a href="https://www.virtualizationhowto.com/2026/09/leaving-vmware-just-got-harder-after-broadcom-pulled-vddk-downloads/">Leaving VMware Just Got Harder After Broadcom Pulled VDDK Downloads - Virtualization Howto</a></li>
<li><a href="https://www.shapeblue.com/broadcom-vddk-download-vmware-to-kvm/">Broadcom Removes VDDK Pages Without Explanation: What You Need to Know - ShapeBlue</a></li>
<li><a href="https://platform9.com/blog/vddk-no-longer-available/">Broadcom Cut Public Access of Virtual Disk Development Kit (VDDK) Overnight • Platform9</a></li>

</ul>
</details>

**Discussion**: Former VMware engineers express sadness over Broadcom's approach, viewing it as extracting value from a declining product. Users share migration experiences, noting that while tools like qemu-img can convert disk images, the lack of VDDK adds friction, though some find Proxmox migration surprisingly painless.

**Tags**: `#VMware`, `#Broadcom`, `#VDDK`, `#virtualization`, `#migration`

---

<a id="item-4"></a>
## [Abusive AI Crawlers Burn 14 CPU Cores on git.kernel.org](https://simonwillison.net/2026/Sep/7/creepy-crawlies/) ⭐️ 7.0/10

Konstantin Ryabitsev reported that abusive crawlers, likely AI-related, now consume more CPU cycles on git.kernel.org than all legitimate access combined, including git clones. At any time, 14 CPU cores across 5 geo-distributed nodes are dedicated solely to rendering git commits as HTML for these scrapers. This highlights the severe operational burden that unregulated web crawlers place on critical open-source infrastructure, potentially degrading performance for legitimate users. It raises concerns for projects like Datasette that serve many crawlable pages, and underscores the need for better crawler management and ethical AI training practices. The report mentions six million requests per day, with only about 2% being legitimate traffic. Ryabitsev also noted that a proof-of-work challenge (like Anubis) only shifts the problem, as abusive crawlers adapt using residential proxies.

rss · Simon Willison · Sep 7, 23:08

**Background**: git.kernel.org is the official Git repository hosting the Linux kernel source code. Web crawlers, including those used by AI companies to gather training data, often scrape public repositories, but excessive and abusive crawling can overwhelm servers. Rendering commits as HTML is a CPU-intensive operation that, when done at scale for scrapers, diverts significant resources from serving legitimate users.

<details><summary>References</summary>
<ul>
<li><a href="https://elsolitario.org/en/2026/08/30/kernel-org-ai-bots-anubis-cpu/">Kernel.org Burns 14 CPU Cores Tracking AI Crawlers</a></li>
<li><a href="https://ettayeb.fr/en/linux/git-kernel-org-ai-crawlers-2026/">AI crawlers burn 20% of git.kernel.org CPU scraping commits ...</a></li>
<li><a href="https://securityonline.info/ai-crawlers-git-kernel/">AI Crawlers Strain git.kernel.org Servers - securityonline.info</a></li>

</ul>
</details>

**Discussion**: The Hacker News discussion likely reflects concern about the impact of AI crawlers on open-source infrastructure, with some suggesting technical mitigations like better bot detection or rate limiting. Others may debate the ethics of AI companies scraping without permission, and the effectiveness of proof-of-work challenges.

**Tags**: `#web crawling`, `#Linux kernel`, `#open source`, `#infrastructure`, `#security`

---

<a id="item-5"></a>
## [OpenAI Chief Scientist Advocates for Defensive AI, Warns Against Reckless Racing](https://simonwillison.net/2026/Sep/7/jakub-pachocki/) ⭐️ 7.0/10

OpenAI Chief Scientist Jakub Pachocki published an essay arguing that powerful, aligned AI is needed for defense against other AI threats, while cautioning that this necessity must not justify reckless development. He stated that building defensive systems will be a primary focus of OpenAI's deployment efforts. This statement from a top AI leader signals a strategic shift toward prioritizing defensive AI applications, potentially influencing industry and policy discussions on AI safety. It reflects the growing tension between the urgency to develop advanced AI for protection and the need to avoid an uncontrolled arms race. Pachocki's comments come from an essay titled 'An Alien Mind' on OpenAI's website, specifically the section on 'scalable defense.' He emphasizes the need to secure infrastructure, protect against rogue agents in real time, and invent new protective measures, while explicitly rejecting the idea of racing forward at all costs.

rss · Simon Willison · Sep 7, 22:26

**Background**: AI alignment refers to ensuring AI systems act in accordance with human intentions and values. The concept of 'scalable defense' suggests using increasingly capable AI to protect against threats from other AI, a topic that has gained prominence as AI capabilities advance. OpenAI has recently launched initiatives like the $1 billion Daybreak program to support cyber defense, aligning with Pachocki's emphasis on defensive AI.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/daybreak-for-frontline-defenders/">Daybreak for Frontline Defenders: $1B to protect essential services | OpenAI</a></li>
<li><a href="https://cyberpress.org/openai-launches-1-billion-daybreak-initiative/">OpenAI Launches $1 Billion Daybreak Initiative for Critical Infrastructure Cyber Defense</a></li>

</ul>
</details>

**Tags**: `#AI safety`, `#OpenAI`, `#AI ethics`, `#AI policy`

---