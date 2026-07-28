---
layout: default
title: "Horizon Summary: 2026-07-28 (EN)"
date: 2026-07-28
lang: en
---

> From 38 items, 3 important content pieces were selected

---

1. [Full takeover of Volvo/Eicher fleet platform disclosed](#item-1) ⭐️ 9.0/10
2. [Kimi K3 2.8T MoE Model Released with MXFP4 Quantization](#item-2) ⭐️ 9.0/10
3. [7.1 Earthquake Strikes Japan, Damages Semiconductor Plants](#item-3) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Full takeover of Volvo/Eicher fleet platform disclosed](https://eaton-works.com/2026/07/27/my-eicher-hack/) ⭐️ 9.0/10

Security researcher published details of a critical vulnerability in VE Commercial Vehicles' My Eicher fleet management platform that allowed full account takeover and control over all users and vehicles, after responsible disclosure went unanswered for weeks. This highlights severe security risks in connected vehicle platforms, where a single flaw could enable remote control of thousands of commercial vehicles, threatening fleet safety and privacy. The vulnerability was reported on November 3, 2025, but after no response, the researcher published on July 27, 2026, noting the primary issue was fixed by November 20, 2025, but without acknowledgment.

hackernews · EatonZ · Jul 27, 15:08 · [Discussion](https://news.ycombinator.com/item?id=49070756)

**Background**: My Eicher is a digital fleet management platform by VE Commercial Vehicles (a Volvo-Eicher joint venture) offering real-time tracking, fuel management, and uptime services. Such platforms are increasingly critical for commercial fleet operations, making their security paramount.

<details><summary>References</summary>
<ul>
<li><a href="https://eaton-works.com/2026/07/27/my-eicher-hack/">Exploiting Volvo/Eicher’s fleet management platform to gain ...</a></li>
<li><a href="https://www.eichertrucksandbuses.com/support-solutions/my-eicher">My Eicher | Fleet Monitoring Platform for Trucks & Buses</a></li>

</ul>
</details>

**Discussion**: Comments expressed concern over EV battery management system security and the dangers of cloud-dependent car functions, with some criticizing the company's unresponsive disclosure process while others praised the researcher's patience.

**Tags**: `#security`, `#automotive`, `#vulnerability`, `#IoT`, `#responsible disclosure`

---

<a id="item-2"></a>
## [Kimi K3 2.8T MoE Model Released with MXFP4 Quantization](https://www.reddit.com/r/LocalLLaMA/comments/1v81qw0/kimi_k3_weights_drop_today_were_deploying_on/) ⭐️ 9.0/10

Moonshot AI released the weights for Kimi K3, a 2.8 trillion parameter Mixture-of-Experts model with 896 experts and 16 active per token, using MXFP4 quantization-aware training. The model is being deployed on A100, H200, and B300 GPUs, with initial memory analysis showing that only B300 nodes can fit the full model in a single node. Kimi K3 is one of the largest open-weight models ever released, pushing the boundaries of MoE scaling and quantization. Its deployment challenges highlight the growing gap between model size and available hardware, and the need for efficient quantization like MXFP4 to make such models practical. The model weights are approximately 1.4 TB in MXFP4 format, requiring at least three 8x A100 nodes or two 8x H200 nodes to load, with no room for KV cache. On A100s, which lack FP4 tensor cores, inference will require dequantization or INT4 kernels, likely resulting in poor performance.

reddit · r/LocalLLaMA · /u/qubridInc · Jul 27, 14:18

**Background**: Mixture-of-Experts (MoE) models use multiple specialized sub-networks (experts) and activate only a subset per token, enabling large total parameters with lower computational cost. MXFP4 is a 4-bit floating-point quantization format standardized by the Open Compute Project, designed for efficient hardware inference. The B300 GPU, with 288 GB of HBM3e memory per GPU, is the only current hardware that can fit the entire K3 model in a single 8-GPU node.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2603.08713">Unveiling the Potential of Quantization with MXFP4 ...</a></li>
<li><a href="https://pantheon.run/learn/nvidia-hgx-b300-specs">NVIDIA HGX B 300 Specs & Datasheet (8- GPU Node) | Pantheon</a></li>

</ul>
</details>

**Discussion**: The Reddit community expressed excitement about the release but also concern over the practical deployment challenges, especially on A100s. Many users discussed the memory requirements and the need for advanced quantization, with some questioning whether running on A100s is worthwhile given the expected performance degradation.

**Tags**: `#LLM`, `#MoE`, `#quantization`, `#hardware`, `#deployment`

---

<a id="item-3"></a>
## [7.1 Earthquake Strikes Japan, Damages Semiconductor Plants](https://www.data.jma.go.jp/multi/quake/quake_detail.html?eventID=20260728163528&lang=en) ⭐️ 8.0/10

A 7.1 magnitude earthquake struck Kumamoto Prefecture, Japan, on July 28, 2026, causing casualties, building collapses, fires, and evacuations at major tech facilities including TSMC, Sony, and Fujifilm. This earthquake disrupts critical semiconductor supply chains, as the affected region hosts key fabrication plants for chips, image sensors, and materials, potentially impacting global electronics production. The earthquake registered a shindo of 7 in parts of Kumamoto, indicating extreme shaking. At least 50 people were hospitalized, 9 missing, 12 houses collapsed, and 7 fires reported, including an explosion at an AEON mall.

hackernews · krembo · Jul 28, 07:44 · [Discussion](https://news.ycombinator.com/item?id=49080664)

**Background**: The Japanese shindo scale measures ground shaking intensity, with 7 being the highest level, typically causing severe damage. The region is still recovering from a previous major earthquake, and the Nankai Trough is a known seismic risk area.

**Discussion**: Community members reported detailed damage: multiple highway bridges snapped, a paper factory chimney collapsed, and TSMC, Sony, and Fujifilm plants were evacuated. Some expressed concern about the region's incomplete recovery from prior quakes and fear of future Nankai Trough earthquakes.

**Tags**: `#earthquake`, `#Japan`, `#disaster`, `#semiconductor`, `#infrastructure`

---