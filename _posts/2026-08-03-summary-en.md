---
layout: default
title: "Horizon Summary: 2026-08-03 (EN)"
date: 2026-08-03
lang: en
---

> From 34 items, 4 important content pieces were selected

---

1. [Qwen3.8-Max: Alibaba's Most Capable Model, Open Weights Coming](#item-1) ⭐️ 8.0/10
2. [China's DFSX Claims 2x Memory Bandwidth of NVIDIA GB200](#item-2) ⭐️ 8.0/10
3. [MiniMax-H3 Omni-Modal Model Released on Hugging Face](#item-3) ⭐️ 8.0/10
4. [Open Letters Debate AI Open Weights and Safety](#item-4) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Qwen3.8-Max: Alibaba's Most Capable Model, Open Weights Coming](https://qwen.ai/blog?id=qwen3.8) ⭐️ 8.0/10

Alibaba's Qwen team announced Qwen3.8-Max, the most capable model in the Qwen family to date, featuring 2.4 trillion parameters with a Mixture-of-Experts architecture. For the first time, they will open-source the weights of a Qwen-Max-class model, with the open weights to be released next week. This release is significant because it marks the first time a Max-class model from Qwen will be open-sourced, potentially democratizing access to top-tier AI capabilities. It could intensify competition in the AI model market, especially against other leading models like Fable 5 and Grok 4.5, and lower the barrier for developers and startups to use advanced AI. Qwen3.8-Max supports a reasoning_effort parameter with three levels (xhigh, medium, low) to adjust reasoning depth and control cost. The model is currently available as a preview, and while it rivals Fable 5 and Grok 4.5 in coding tests, it has a notable speed limitation.

hackernews · ai2027 · Aug 3, 02:16 · [Discussion](https://news.ycombinator.com/item?id=49150470)

**Background**: Qwen is a family of large language models developed by Alibaba, known for both open-weight and API-based offerings. Open-weight models provide the trained model weights publicly, allowing developers to self-host and fine-tune them, which promotes transparency and innovation. Qwen3.8-Max is a flagship model with a Mixture-of-Experts architecture, which uses multiple specialized sub-networks to improve efficiency and performance.

<details><summary>References</summary>
<ul>
<li><a href="https://www.eesel.ai/blog/qwen38-max-review">Qwen 3.8 Max review: Alibaba's 2.4T flagship, tested (2026)</a></li>
<li><a href="https://docs.qwencloud.com/changelog/models">Model releases - QwenCloud</a></li>
<li><a href="https://thomas-wiegold.com/blog/qwen-3-8-max-review/">Qwen3.8-Max Review: I Tested Alibaba's 2.4T Model</a></li>

</ul>
</details>

**Discussion**: Community comments express excitement about the open-weight release, especially for the smaller Qwen3.8-27B model, which is praised as one of the best local models. Some users are concerned about cost, hoping the API pricing will be competitive with DeepSeek, while others humorously suggest that a model's ability to explain its own pricing page is a key benchmark. There is also skepticism about the timing of such announcements relative to OpenAI and Anthropic going public.

**Tags**: `#AI`, `#LLM`, `#Open Source`, `#Qwen`, `#Machine Learning`

---

<a id="item-2"></a>
## [China's DFSX Claims 2x Memory Bandwidth of NVIDIA GB200](https://www.reddit.com/r/LocalLLaMA/comments/1vduej3/chinas_dfsx_offers_2x_the_memory_bandwidth_of/) ⭐️ 8.0/10

DFSX, a Chinese chipmaker, announced its TY64 SuperNode with DF2000 chips, claiming a memory bandwidth of 960TB/s, which is double the 576TB/s of NVIDIA's GB200 NVL72 system. The chip uses a 14nm process and a unique vertical compute-memory tower design that skips microbumps. This development could reshape the competitive landscape in AI hardware, as China aims to challenge NVIDIA's dominance despite US export controls. If the claims hold, it may offer a viable alternative for AI training and inference, potentially lowering costs and increasing supply chain diversity. The DFSX TY64 SuperNode is built from 14nm DF2000 chips and achieves 960TB/s memory bandwidth, compared to 576TB/s for NVIDIA's GB200 NVL72. The design uses vertical compute-memory towers that skip microbumps, potentially improving manufacturing yield and performance. However, detailed benchmarks and real-world performance data are not yet available.

reddit · r/LocalLLaMA · /u/MundanePercentage674 · Aug 2, 21:39

**Background**: Memory bandwidth is critical for AI workloads, as it determines how fast data can be fed to compute units. NVIDIA's GB200 uses HBM3e memory and offers 576TB/s per rack, while DFSX's approach uses a 14nm process, which is less advanced than NVIDIA's 4nm, but compensates with a novel architecture. China has been investing heavily in domestic semiconductor alternatives due to US export restrictions on advanced chips and equipment.

<details><summary>References</summary>
<ul>
<li><a href="https://wccftech.com/chinas-dfsx-offers-2x-the-memory-bandwidth-of-nvidias-gb200-nvl72-system-with-a-14nm-supernode-that-skips-microbumps-for-vertical-compute-memory-towers/">China's DFSX Offers 2x The Memory Bandwidth Of NVIDIA's ... - Wccftech</a></li>
<li><a href="https://hellochinatech.com/p/dfsx-14nm-ai-chip-wager">Can China's 14nm AI Chip Challenge 4nm Designs?</a></li>
<li><a href="https://www.nexgencloud.com/blog/case-studies/nvidia-gb200-user-guide-specs-features-and-use-cases">NVIDIA GB200 User Guide: Specs, Features and Use Cases</a></li>

</ul>
</details>

**Tags**: `#AI hardware`, `#memory bandwidth`, `#China`, `#NVIDIA`, `#semiconductors`

---

<a id="item-3"></a>
## [MiniMax-H3 Omni-Modal Model Released on Hugging Face](https://www.reddit.com/r/LocalLLaMA/comments/1ve1mvh/minimaxh3_now_on_huggingface/) ⭐️ 8.0/10

MiniMax has released MiniMax-H3, a general-purpose omni-modal generative system, on Hugging Face. It supports unified understanding and generation across text, images, video, and audio, with the ability to generate up to 15-second 2K video with native stereo audio. This release marks a significant advancement in multimodal AI, as it combines understanding and generation across multiple modalities in a single model, potentially simplifying workflows and enabling new applications. It also signals a trend toward open-sourcing powerful omni-modal models, which could accelerate innovation in the community. MiniMax-H3 can generate video with native stereo audio at resolutions up to 2K and durations up to 15 seconds. It can process up to 9 images, 3 video clips, and 3 audio tracks in a single context, and its task-generalization-oriented design enables strong performance in following complex multimodal instructions even at the pre-training stage.

reddit · r/LocalLLaMA · /u/Mobile-Pumpkin7944 · Aug 3, 03:06

**Background**: Omni-modal models are AI systems that can process and generate multiple types of data, such as text, images, video, and audio, within a unified framework. Traditional models often specialize in one modality, but omni-modal models aim to integrate understanding and generation across all modalities, enabling more natural and comprehensive interactions. MiniMax-H3 builds on this concept, offering a single system that can handle diverse inputs and outputs.

<details><summary>References</summary>
<ul>
<li><a href="https://www.minimax.io/blog/minimax-h3">MiniMax H3: An Open Model Breaking the Boundaries Between Tasks and Modalities - MiniMax Research | MiniMax</a></li>
<li><a href="https://www.marktechpost.com/2026/08/01/minimax-releases-minimax-h3-an-omni-modal-video-model-that-generates-15-second-2k-clips-with-native-stereo-audio/">MiniMax Releases MiniMax H3: An Omni-Modal Video Model That Generates 15-Second 2K Clips With Native Stereo Audio - MarkTechPost</a></li>
<li><a href="https://huggingface.co/MiniMaxAI/MiniMax-H3">MiniMaxAI/MiniMax-H3 · Hugging Face</a></li>

</ul>
</details>

**Tags**: `#multimodal`, `#generative AI`, `#Hugging Face`, `#video generation`, `#AI model release`

---

<a id="item-4"></a>
## [Open Letters Debate AI Open Weights and Safety](https://simonwillison.net/2026/Aug/2/open-letters/#atom-everything) ⭐️ 7.0/10

Microsoft released an open letter titled 'Open Weights and American AI Leadership' on July 24, 2026, signed by 235 companies including NVIDIA, Amazon, and later OpenAI, advocating for open-weight AI models. In response, Anthropic published its own position on open-weights models three days later, and on July 28, 'Pacing the Frontier' was released with signatures from 1,324 employees of frontier AI companies. These letters highlight a significant policy debate about AI safety and open-source models, with major industry players taking opposing stances. The outcome could shape US government regulations on AI development, affecting innovation, competition, and global AI leadership. The Microsoft letter explicitly supports distillation, a technique where models train on outputs from other models, arguing it is a legitimate development method. Notably, Anthropic did not sign the letter and instead called for a crackdown on industrial-scale distillation operations, while stating it has never advocated for a ban on open-weights models.

rss · Simon Willison · Aug 2, 04:16

**Background**: Open-weight AI models are models whose trained parameters are publicly released, allowing anyone to use, modify, and study them, in contrast to closed models like GPT-4. The debate centers on balancing the benefits of transparency and innovation against risks of misuse, such as cyberattacks or biological attacks. The US government has previously taken actions against certain models over safety concerns, such as the directive to suspend access to Claude Fable 5.

<details><summary>References</summary>
<ul>
<li><a href="https://www.microsoft.com/en-us/corporate-responsibility/topics/open-weight/">Open Weights and American AI Leadership - microsoft.com</a></li>
<li><a href="https://www.anthropic.com/news/position-open-weights-models">Our position on open-weights models \ Anthropic</a></li>
<li><a href="https://www.npr.org/2026/05/31/nx-s1-5816391/ai-safety-concerns-danger-open-weight-models-risks">Why open-weight models without guardrails are a AI safety risk : NPR</a></li>

</ul>
</details>

**Tags**: `#AI`, `#open source`, `#policy`, `#industry`, `#Simon Willison`

---