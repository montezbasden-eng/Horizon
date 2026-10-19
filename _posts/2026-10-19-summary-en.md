---
layout: default
title: "Horizon Summary: 2026-10-19 (EN)"
date: 2026-10-19
lang: en
---

> From 32 items, 3 important content pieces were selected

---

1. [Together Computer Releases Hybrid Reasoning Agents That Think in Latent Space](#item-1) ⭐️ 8.0/10
2. [RepRapMicron: Open-Source Micron-Scale 3D Printer Project](#item-2) ⭐️ 8.0/10
3. [Ken Shirriff Explains Intel 8087 Floating-Point Addition and Subtraction Microcode](#item-3) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Together Computer Releases Hybrid Reasoning Agents That Think in Latent Space](https://arxiv.org/abs/2610.18861) ⭐️ 8.0/10

Together Computer has released Hybrid Reasoning Agents, a system where LLM agents perform reasoning in a continuous latent space while acting through text, with open code, models, and evaluations available on GitHub, Hugging Face, and arXiv. The release includes an 8B agentic model built on Qwen3-8B-Base and trained with HybridSFT followed by HybridRL. This work pushes toward a new paradigm where models reason internally in latent space rather than generating verbose chain-of-thought text, potentially improving efficiency and capability for agentic tasks. It also sparks debate on interpretability and safety, since latent reasoning is harder to monitor than explicit thinking tokens. The 8B agentic checkpoint's latent thoughts are claimed to remain directly interpretable, with every latent step readable as pseudo-text. However, a community member reproduced a failure mode where the quantized GGUF model got stuck in an infinite thinking loop on a simple question, highlighting reliability concerns.

hackernews · allinonai · Oct 18, 20:48 · [Discussion](https://news.ycombinator.com/item?id=50145337)

**Background**: Latent space reasoning refers to models performing intermediate computation in continuous hidden states instead of decoding them into words, as explored in approaches like Coconut. Hybrid agents combine this with text-based action, aiming to keep the benefits of interpretable outputs while reducing the cost of verbose reasoning. Together Computer is an AI cloud platform that also develops open models and research.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/togethercomputer/HybridAgent">GitHub - togethercomputer/HybridAgent</a></li>
<li><a href="https://huggingface.co/togethercomputer/HybridAgent-8B-Agentic">togethercomputer/HybridAgent-8B-Agentic · Hugging Face</a></li>
<li><a href="https://arxiv.org/pdf/2412.06769">Training Large Language Models to Reason in a Continuous Latent ...</a></li>

</ul>
</details>

**Discussion**: Commenters debated safety and interpretability, noting that latent reasoning may increase capacity for deception and complicate monitoring compared to explicit thinking tokens. One user reported that a quantized GGUF model got stuck in an endless thinking loop on a simple question, while others discussed architectural alternatives and potential speedups.

**Tags**: `#LLM agents`, `#latent reasoning`, `#AI safety`, `#interpretability`, `#research`

---

<a id="item-2"></a>
## [RepRapMicron: Open-Source Micron-Scale 3D Printer Project](https://github.com/VikOlliver/RepRapMicron/wiki) ⭐️ 8.0/10

RepRapMicron (μRepRap) is an open-source project extending the RepRap 3D printer lineage to achieve micron-scale fabrication, with a positioning accuracy of a few microns and feature sizes of 10–20 μm using a computer-controlled flexure motion system. If successful, this project could democratize microchip manufacturing by making micron-scale fabrication accessible to hobbyists and small communities, potentially breaking the semiconductor industry's fixation on silicon and enabling independent innovation in microelectronics. The printer uses flexure mechanisms to eliminate friction and backlash, works with standard 3D printer and CNC controllers, and aims to be built by average enthusiasts; however, challenges remain in print quality for larger objects and replication of the printer itself at 1/1000 scale is still a goal.

hackernews · RobotToaster · Oct 18, 13:48 · [Discussion](https://news.ycombinator.com/item?id=50141076)

**Background**: RepRap is a project to develop low-cost 3D printers that can print most of their own components, released under free software licenses. Microfabrication traditionally involves fabricating structures at micrometre scales, historically used for integrated circuit fabrication and requiring expensive industrial-grade equipment. RepRapMicron aims to bring this capability to the desktop.

<details><summary>References</summary>
<ul>
<li><a href="https://reprap.org/wiki/RepRapMicron">RepRapMicron - RepRap GitHub - VikOlliver/RepRapMicron: μRepRap - A 3D printer ... Nail Gel and Acupuncture Needles: How a DIY 3D Printer Hit 1 ... Shrinking the Factory: Meet RepRapMicron, the Open-Source ... RepRapMicron PIKA: 1μm Positioning, Replication Still a Goal RepRapMicron: Exploring Micro-Manufacturing via Precision ... RepRapMicron Micron Scale 3D Printer by vik - Thingiverse</a></li>
<li><a href="https://github.com/VikOlliver/RepRapMicron">GitHub - VikOlliver/RepRapMicron: μRepRap - A 3D printer ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/RepRap">RepRap - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters drew historical parallels to precision engineering breakthroughs of the late 1790s, such as Ramsden's dividing engine and Maudslay's thread-cutting lathe, suggesting this could be a similar transformative moment. Some expressed excitement about eventually making their own RAM or enabling cheap and sustainable printing of chip designs, while others questioned the feasibility of a 1/1000 self-replicating printer.

**Tags**: `#3D printing`, `#microfabrication`, `#open hardware`, `#RepRap`, `#precision engineering`

---

<a id="item-3"></a>
## [Ken Shirriff Explains Intel 8087 Floating-Point Addition and Subtraction Microcode](https://www.righto.com/2026/10/8087-addition-subtraction-microcode.html) ⭐️ 8.0/10

Ken Shirriff published a new article on the Intel 8087 coprocessor, detailing how floating-point addition and subtraction are implemented in microcode, including numerous special cases. The article explains the chip's adder, shifter, and exponent converter circuitry and notes that the 8087 sped up addition by almost 100x over the 8086. The deep dive provides rare insight into how early hardware implemented IEEE floating-point arithmetic, which remains foundational to modern computing. It also highlights the historical significance of the 8087 as the first floating-point coprocessor for the 8086 line and its lasting influence on later x87 math coprocessors. The 8087, announced in 1980, used complicated algorithms implemented in microcode to accurately compute functions such as square roots, tangents, and exponentials. The article focuses specifically on the microcode and circuitry for addition and subtraction, covering the special cases that arise in floating-point operations.

hackernews · pwg · Oct 18, 16:20 · [Discussion](https://news.ycombinator.com/item?id=50142449)

**Background**: The Intel 8087 was the first floating-point coprocessor for the 8086 microprocessor line, designed to accelerate arithmetic operations like addition, subtraction, multiplication, division, and square root. It was directly connected to the address and data buses and monitored instructions beginning with the '11011' prefix. Microcode is low-level code inside the chip that controls these operations, and Ken Shirriff has previously examined the 8087's microcode ROM by opening up the chip and imaging it under a microscope.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Intel_8087">Intel 8087 - Wikipedia</a></li>
<li><a href="https://www.righto.com/2026/10/8087-addition-subtraction-microcode.html">Inside the Intel 8087 chip: floating-point addition and ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Floating-point_unit">Floating-point unit - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters expressed admiration for the 8087's capabilities, with Walter Bright sharing an anecdote about persuading Microsoft to preserve 8087 registers during context switches in early Win32. Others noted the contrast between the 1980 chip's 80-bit floating-point support and modern microcontrollers that still lack floating-point units, and thanked Ken Shirriff for his detailed technical writing.

**Tags**: `#Intel 8087`, `#floating-point`, `#microcode`, `#computer history`, `#hardware`

---