---
layout: default
title: "Horizon Summary: 2026-10-18 (EN)"
date: 2026-10-18
lang: en
---

> From 35 items, 3 important content pieces were selected

---

1. [DeepSeek releases V4.1-Flash-1017, an open model that beats Sol 5.6 on most coding benchmarks](#item-1) ⭐️ 8.0/10
2. [Solar overtakes nuclear in global electricity generation for the first time](#item-2) ⭐️ 8.0/10
3. [Xolotl runs 552B DeepSeek-V4.1-Flash on a single RTX 4090 at 27 tok/s](#item-3) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [DeepSeek releases V4.1-Flash-1017, an open model that beats Sol 5.6 on most coding benchmarks](https://huggingface.co/deepseek-ai/DeepSeek-V4.1-Flash-1017) ⭐️ 8.0/10

DeepSeek released DeepSeek-V4.1-Flash-1017, a minor dated update to DeepSeek-V4.1-Flash, which delivers substantial improvements across reasoning, coding, agentic tasks, and visual understanding. According to DeepSeek's own news page, the new version scores significantly higher on multiple coding benchmarks, beating Sol 5.6 on 10 out of 11 benchmarks. This release strengthens the position of open-weight models against proprietary leaders like OpenAI's Sol and Anthropic's Claude, giving developers a fast, openly licensed alternative for coding and agentic workflows. It also fuels the debate about regulatory hurdles and the value of a diverse AI ecosystem. The model is an open-weight release under the MIT license, available on Hugging Face and via OpenRouter, and is described as a minor update rather than a new architecture. Community testing suggests it is fast (high tokens per second, low time-to-first-token) and transparent (visible chain-of-thought), but in one real-world code review it took 20 minutes to find one relevant P1 issue, compared to about 5 minutes for Sol 5.6.

hackernews · theykk · Oct 17, 08:21 · [Discussion](https://news.ycombinator.com/item?id=50129045)

**Background**: DeepSeek is a Chinese AI company known for releasing open-weight large language models that compete with proprietary offerings. V4.1-Flash is its fast, lightweight model line, and the 1017 suffix indicates a dated update released on October 17. Sol 5.6 refers to a version of OpenAI's GPT-5.6 Sol model, which leads on several agentic benchmarks such as Terminal-Bench 2.1 and BrowseComp. OpenRouter is a platform that provides a unified API for accessing many models, which makes it easy for developers to try new releases like this one.

<details><summary>References</summary>
<ul>
<li><a href="https://the-agent-report.com/2026/07/gpt-5-6-sol-terra-luna-benchmarks-pricing-analysis/">GPT-5.6 Sol, Terra, Luna: Full Benchmark Analysis and Which ...</a></li>

</ul>
</details>

**Discussion**: Hacker News commenters largely agree that DeepSeek feels better in practice due to faster token throughput and lower latency, plus the openness of visible chain-of-thought and fewer content blocks. Some note that while it beats Sol 5.6 on most benchmarks, Sol 6.1 is the latest and still leads in some real-world agent tests, and one commenter argues that models like this are why OpenAI and Anthropic want regulatory hurdles.

**Tags**: `#LLM`, `#DeepSeek`, `#coding benchmarks`, `#model release`, `#AI agents`

---

<a id="item-2"></a>
## [Solar overtakes nuclear in global electricity generation for the first time](https://www.pv-magazine.com/2026/09/29/solar-surpasses-nuclear-power-globally-for-first-time/) ⭐️ 8.0/10

For the first time, solar power has generated more electricity globally than nuclear power, with solar capacity rising 27% year on year to 2,383 GW while nuclear capacity grew only 1.5 GW to 399.5 GW. Wind is also on the verge of surpassing nuclear, and from March 2025 through June 2026 either solar or wind individually out-generated nuclear every month. This milestone marks a structural shift in the global power mix, showing that rapidly scalable renewables can outpace established baseload nuclear despite solar's much lower capacity factor. It signals accelerating decarbonization of electricity and puts pressure on grids and storage to handle variable generation. The comparison is based on actual generated terawatt-hours, not installed capacity; nuclear's capacity factor is near 100% versus roughly 20-30% for solar, so solar needed far more installed capacity to lead. The next major milestone, solar surpassing hydroelectric generation, is several years away at current growth rates.

hackernews · xbmcuser · Oct 17, 14:01 · [Discussion](https://news.ycombinator.com/item?id=50131256)

**Background**: Capacity factor is the ratio of actual electricity produced over a period to the maximum possible output if a plant ran at full power continuously; nuclear plants run near full output, while solar only produces during daylight and at lower efficiency. Global electricity generation is still dominated by fossil fuels at about 57%, with solar and wind each now contributing nearly as much as nuclear. Solar PV converts sunlight directly into electricity via the photovoltaic effect in semiconductor cells.

<details><summary>References</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=21035212">Solar across ANY area has intermittency issues. | Hacker News</a></li>
<li><a href="https://www.linkedin.com/posts/sergio-magdaleno-bbb187208_ranked-the-worlds-biggest-electricity-sources-activity-7462134048556003328-cUBo">Fossil Fuels Dominate Global Electricity Mix in 2025 | LinkedIn</a></li>
<li><a href="https://ourworldindata.org/grapher/solar-energy-generation-vs-capacity">Solar energy generation vs . capacity | Our World in Data</a></li>

</ul>
</details>

**Discussion**: Commenters highlighted that the milestone reflects actual generated TWh despite nuclear's higher capacity factor, and noted wind is close behind while solar races ahead. Some lamented nuclear's stagnation as lost decades of progress, while others stressed that clean energy deployment must accelerate further to replace fossil fuels entirely, including hydrocarbons used as chemical feedstocks.

**Tags**: `#energy`, `#solar`, `#nuclear`, `#climate-tech`, `#renewables`

---

<a id="item-3"></a>
## [Xolotl runs 552B DeepSeek-V4.1-Flash on a single RTX 4090 at 27 tok/s](https://www.reddit.com/r/LocalLLaMA/comments/1x8m0jj/xolotl_strata_based_deepseekv41flash_552b_on_a/) ⭐️ 8.0/10

A developer released Xolotl, a Strata-based inference engine that runs the full 552B-parameter DeepSeek-V4.1-Flash model on a single RTX 4090 (24GB) with 90GB DDR4 RAM and an NVMe drive, achieving ~27 tok/s decode and 180–320 tok/s prefill with 512K context. The engine also supports GLM-5.3-Flash, Qwen3.8-Flash-Next, and Qwen3.8-27B, and an uncensored 1017 quant is expected in a couple of days. This demonstrates that massive Mixture-of-Experts models can be run on consumer-grade hardware through expert offloading, potentially democratizing access to frontier-scale LLMs for local users. It also shows a community project achieving practical throughput with concrete benchmarks, which could inspire further optimization in the local LLM ecosystem. The engine spreads weights across VRAM, pinned RAM, and NVMe, dynamically pulling only the experts needed per token; it reports 21/21 on HumanEval, 10/10 tool calls, and 3/3 agentic bug-fix loops through the real server with thinking enabled. The upcoming 1017 quant is a 510GB download that requires full recalibration and quantization, not a quick patch, and the current uncensored quant is 152 GiB.

reddit · r/LocalLLaMA · /u/indrasmirror · Oct 17, 21:40

**Background**: Strata is an open-source inference engine that runs large Mixture-of-Experts (MoE) models on consumer PCs by offloading expert weights to system RAM and NVMe, treating VRAM as a cache. MoE models activate only a subset of experts per token, so offloading inactive experts to slower storage can make huge models fit on limited hardware. GSQ (Gumbel-Softmax Quantization) is a post-training scalar quantization method that learns per-coordinate bit depths to reduce model size with high accuracy.

<details><summary>References</summary>
<ul>
<li><a href="https://stratallm.org/">Strata LLM – Run 125B+ MoE Models on 12GB VRAM Consumer GPUs ...</a></li>
<li><a href="https://github.com/Niko1221/Strata">GitHub - Niko1221/Strata: Qwen3.8-Flash-Next on any consumer ...</a></li>
<li><a href="https://apxml.com/courses/mixture-of-experts-advanced-implementation/chapter-4-efficient-moe-inference/expert-offloading">MoE Expert Offloading to CPU/NVMe - apxml.com</a></li>

</ul>
</details>

**Tags**: `#local-llm`, `#inference-engine`, `#model-offloading`, `#mixture-of-experts`, `#quantization`

---