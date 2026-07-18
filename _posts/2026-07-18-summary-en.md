---
layout: default
title: "Horizon Summary: 2026-07-18 (EN)"
date: 2026-07-18
lang: en
---

> From 42 items, 5 important content pieces were selected

---

1. [First Atmosphere Found on Earth-like Planet in Habitable Zone](#item-1) ⭐️ 8.0/10
2. [TP-Link Kasa cameras leak home GPS via unauthenticated UDP](#item-2) ⭐️ 8.0/10
3. [Practical SQLite Tips: .expert Mode and AWS Backups](#item-3) ⭐️ 8.0/10
4. [Anthropic makes Claude Fable 5 permanent in subscription plans](#item-4) ⭐️ 8.0/10
5. [NVIDIA NeMo Automodel & Diffusers for Scalable Fine-Tuning](#item-5) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [First Atmosphere Found on Earth-like Planet in Habitable Zone](https://www.bbc.com/news/articles/cy4kdd1e0ejo) ⭐️ 8.0/10

JWST has confirmed the presence of an atmosphere on LHS 1140b, a rocky super-Earth in the habitable zone of a red dwarf star 48 light-years away, marking the first such detection for an Earth-like planet in a habitable zone. This discovery challenges previous assumptions that rocky planets around red dwarfs cannot retain atmospheres due to intense stellar activity, and opens a new frontier for studying potentially habitable exoplanets. LHS 1140b is about 5.6 times Earth's mass and 70% larger in radius, with a density suggesting it may be an ocean world with 9-19% water by mass; JWST's emission spectroscopy ruled out a mini-Neptune interpretation.

hackernews · neversaydie · Jul 17, 14:06 · [Discussion](https://news.ycombinator.com/item?id=48947560)

**Background**: Red dwarfs are cooler and smaller than the Sun, so their habitable zones are much closer, exposing planets to intense stellar flares and radiation that can strip atmospheres. LHS 1140b was discovered in 2017 by the MEarth Project and has been a prime target for atmospheric studies due to its transiting nature.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/LHS_1140_b">LHS 1140 b</a></li>
<li><a href="https://science.nasa.gov/exoplanet-catalog/lhs-1140-b/">LHS 1140 b - NASA Science</a></li>
<li><a href="https://www.bbc.com/news/articles/cy4kdd1e0ejo">First atmosphere found around Earth-like planet LHS 1140b</a></li>

</ul>
</details>

**Discussion**: Commenters debated whether LHS 1140b is truly Earth-like, with some initially suspecting it might be a mini-Neptune being boiled off, but JWST data ruled that out. Others discussed future technologies like solar lens telescopes and near-light-speed propulsion to explore such planets, and reflected on the Fermi paradox and the narrow window for detecting intelligent life.

**Tags**: `#exoplanets`, `#JWST`, `#astronomy`, `#habitable zone`, `#atmosphere`

---

<a id="item-2"></a>
## [TP-Link Kasa cameras leak home GPS via unauthenticated UDP](https://github.com/BadChemical/IoT-Vulnerability-Research-Public/blob/main/TP-Link_Kasa_EC71/Kasa_EC71.md) ⭐️ 8.0/10

A security researcher disclosed that TP-Link Kasa cameras expose precise home GPS coordinates via a single unauthenticated UDP packet, a vulnerability publicly known since 2020 but still unpatched in some devices. This vulnerability poses a serious privacy risk, as an attacker on the same local network can pinpoint a home's location without any authentication, undermining the security of IoT devices that are often deployed in sensitive environments. The vulnerability is tracked as CVE-2026-13230 and affects multiple Kasa camera models; the researcher reported that TP-Link's beta patch bricked the test device, and a factory reset does not clear previous owner data.

hackernews · BadChemical · Jul 17, 21:42 · [Discussion](https://news.ycombinator.com/item?id=48952565)

**Background**: UDP is a connectionless network protocol that does not establish a secure handshake, making it vulnerable to spoofing and unauthorized access if not properly authenticated. IoT devices often use UDP for low-latency communication, but without encryption or authentication, they can leak sensitive data. The TP-Link Kasa cameras respond to a specific UDP packet with GPS coordinates, which should have required authentication.

<details><summary>References</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=48952565">TP-Link Kasa cameras leaked home GPS via unauthenticated UDP for 6 years</a></li>
<li><a href="https://byteiota.com/tp-link-kasa-your-security-camera-leaked-home-gps/">TP-Link Kasa: Your Security Camera Leaked Home GPS | byteiota</a></li>
<li><a href="https://www.cardinalpeak.com/blog/using-udp-in-internet-of-things-devices">Using UDP in Internet of Things Devices - Contract Engineering, Product Design & Development Company - Cardinal Peak</a></li>

</ul>
</details>

**Discussion**: Some commenters noted that the vulnerability is limited to LAN access, reducing its severity, while others emphasized that IoT devices should never communicate over the public internet. The researcher expressed frustration with the disclosure process, including a bricked device and a vendor that mischaracterized the vulnerability.

**Tags**: `#IoT security`, `#privacy`, `#vulnerability disclosure`, `#TP-Link`, `#GPS leak`

---

<a id="item-3"></a>
## [Practical SQLite Tips: .expert Mode and AWS Backups](https://jvns.ca/blog/2026/07/17/learning-about-running-sqlite/) ⭐️ 8.0/10

Julia Evans shares practical tips for running SQLite, including using the .expert command to get index recommendations and backing up databases to AWS S3. These tips help developers optimize SQLite performance and simplify backup workflows, making SQLite more accessible for production and personal projects. The .expert mode in the SQLite CLI analyzes queries and suggests indexes to improve performance. For backups, tools like s3-credentials can generate scoped AWS credentials for secure S3 uploads.

hackernews · surprisetalk · Jul 17, 17:45 · [Discussion](https://news.ycombinator.com/item?id=48950122)

**Background**: SQLite is a lightweight, embedded database engine widely used in applications. The .expert command is a built-in feature of the SQLite command-line shell that recommends indexes based on query analysis. Backing up SQLite databases to cloud storage like AWS S3 ensures data durability and disaster recovery.

<details><summary>References</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=48950122">Learning a few things about running SQLite | Hacker News</a></li>
<li><a href="https://sqlite.org/cli.html">Command Line Shell For SQLite</a></li>
<li><a href="https://github.com/ridl-uta/DatabaseBackupCLI">GitHub - ridl-uta/DatabaseBackupCLI · GitHub</a></li>

</ul>
</details>

**Discussion**: The Hacker News discussion praises Julia's authentic exploration style, contrasting it with AI-generated content. Users share additional tips, such as using zstd compression for backups and the s3-credentials tool for simplified AWS authentication.

**Tags**: `#SQLite`, `#database`, `#optimization`, `#backup`, `#tooling`

---

<a id="item-4"></a>
## [Anthropic makes Claude Fable 5 permanent in subscription plans](https://simonwillison.net/2026/Jul/18/claude-make-fable-5-permanent/#atom-everything) ⭐️ 8.0/10

Anthropic reversed its decision to remove Claude Fable 5 from subscription plans, announcing that starting July 20, Fable 5 will be included in all Max and Team Premium plans at 50% of limits, and Pro and Team Standard users will receive a one-time $100 credit. This reversal highlights the intense competitive pressure from rivals like GPT-5.6 Sol and Kimi 3, forcing Anthropic to keep its best model accessible to subscribers to retain users. It signals a shift in AI pricing strategy where top-tier models become a standard subscription feature rather than an add-on. The original plan to remove Fable 5 from subscriptions was driven by compute capacity concerns, but competitive dynamics made it untenable. Fable 5 is a Mythos-class model, and GPT-5.6 Sol outperforms it on coding benchmarks while costing less.

rss · Simon Willison · Jul 18, 06:00

**Background**: Claude Fable 5 is a publicly available version of Anthropic's Mythos-class model, designed for autonomous knowledge work and coding. It was previously slated to be removed from subscription plans and made available only via API pricing, which would have required users to pay per-token fees. The decision to reverse course came after the release of GPT-5.6 Sol, which set a new state of the art on coding benchmarks, and the emergence of Kimi 3, another competitive model.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/news/claude-fable-5-mythos-5">Claude Fable 5 and Claude Mythos 5 \ Anthropic</a></li>
<li><a href="https://openai-dotcom-git-main-openai.vercel.app/index/gpt-5-6/">GPT - 5 . 6 : Frontier intelligence that scales with your ambition | OpenAI</a></li>

</ul>
</details>

**Discussion**: The community expressed relief that the 'Fablepocalypse' is over, with many noting that paying $100-200/month for a plan without the best model was unreasonable. Some wondered if Anthropic would need to scale back training to free up GPUs for serving Fable 5.

**Tags**: `#AI`, `#Anthropic`, `#Claude`, `#subscription`, `#competition`

---

<a id="item-5"></a>
## [NVIDIA NeMo Automodel & Diffusers for Scalable Fine-Tuning](https://huggingface.co/blog/nvidia/scale-diffusers-finetuning-nemo-automodel) ⭐️ 7.0/10

NVIDIA NeMo Automodel now integrates with Hugging Face Diffusers to enable scalable fine-tuning of video and image generation models. This collaboration allows users to leverage distributed training for diffusion models at scale. This integration addresses the practical need for efficient large-scale fine-tuning of generative AI models, which is critical for adapting pre-trained models to custom domains. It lowers the barrier for enterprises and researchers to fine-tune state-of-the-art video and image models without building complex training infrastructure. NeMo Automodel is a PyTorch DTensor-native SPMD open-source training library that provides day-0 Hugging Face model support. It supports training and fine-tuning of models accessible through Hugging Face Transformer AutoModel classes, including diffusion models from Diffusers.

rss · Hugging Face Blog · Jul 17, 15:57

**Background**: Fine-tuning large generative models typically requires significant computational resources and specialized infrastructure. NVIDIA NeMo Automodel simplifies this by providing a distributed training library that scales across multiple GPUs, while Hugging Face Diffusers offers a wide range of pre-trained diffusion models for image and video generation. The combination enables users to fine-tune these models efficiently at scale.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/nvidia-nemo/automodel">GitHub - NVIDIA-NeMo/Automodel: 🚀 Pytorch Distributed native training library for LLMs/VLMs with OOTB Hugging Face support</a></li>
<li><a href="https://docs.nvidia.com/nemo/automodel/latest/index.html">NeMo AutoModel Documentation | NVIDIA NeMo AutoModel</a></li>
<li><a href="https://huggingface.co/docs/diffusers/index">Diffusers · Hugging Face</a></li>

</ul>
</details>

**Tags**: `#fine-tuning`, `#NVIDIA NeMo`, `#Diffusers`, `#scalability`, `#generative AI`

---