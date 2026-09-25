---
layout: default
title: "Horizon Summary: 2026-09-25 (EN)"
date: 2026-09-25
lang: en
---

> From 51 items, 4 important content pieces were selected

---

1. [F-Droid 2.0 Launches Major Redesign, Phases Out Privileged Extension](#item-1) ⭐️ 8.0/10
2. [Google's Project Suncatcher to Put ML Infrastructure in Space](#item-2) ⭐️ 8.0/10
3. [Apple Pulls Advanced Data Protection in the UK, Creating Two-Tier Encryption](#item-3) ⭐️ 8.0/10
4. [Liquid AI's LFM2.5-VL-DSpark Speeds Up Vision-Language Models](#item-4) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [F-Droid 2.0 Launches Major Redesign, Phases Out Privileged Extension](https://f-droid.org/2026/09/24/f-droid-2.0-a-new-chapter-for-android-freedom.html) ⭐️ 8.0/10

F-Droid released version 2.0, described as its largest app update in over a decade, featuring a complete redesign of the official client and full support for Android's session installer. This means F-Droid 2.0 will no longer use the F-Droid Privileged Extension (FPE) even when it is installed, enabling background updates on recent Android versions without it. As one of the most widely used open-source Android app stores, F-Droid's overhaul affects a large community of privacy-conscious and free-software users, and the FPE phase-out removes a long-standing configuration pain point. The release also lands amid growing concern over Google's planned Android developer verification requirements, making the future of independent app distribution a central question. The redesign drew immediate scrutiny from commenters, who pointed out visual glitches such as a broken line wrap in the first screenshot and criticized the design ethos for lacking clear visual separation between sections and tappable elements. The shift to the session installer is the key technical change that makes FPE unnecessary for background updates.

hackernews · daveoc64 · Sep 24, 15:26 · [Discussion](https://news.ycombinator.com/item?id=49831968)

**Background**: F-Droid is a free and open-source app repository and client for Android that distributes only FOSS applications, serving as an alternative to Google Play. The F-Droid Privileged Extension (FPE) was a system-level component that allowed F-Droid to install and update apps without user interaction, but it required root access or a custom ROM to set up, which many users found difficult. Google has announced rules requiring Android app developers to register with the company even for apps distributed outside the Play Store, raising fears of a platform lockdown.

<details><summary>References</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=49831968">F - Droid 2 . 0 : A New Chapter for Android Freedom | Hacker News</a></li>
<li><a href="https://memedata.com/post/147740">F - Droid 2 . 0</a></li>
<li><a href="https://keepandroidopen.org/">Keep Android Open</a></li>

</ul>
</details>

**Discussion**: Commenters welcomed the overhaul and the FPE phase-out, with one GrapheneOS user saying they had switched to Droid-ify because F-Droid's UI was terrible and FPE was painful to configure. Others were sharply critical of the new design's lack of visual hierarchy and tappable affordances, and several raised concerns about what F-Droid's future looks like once Google's lockdown takes effect next year.

**Tags**: `#F-Droid`, `#Android`, `#open-source`, `#app-store`, `#UI/UX`

---

<a id="item-2"></a>
## [Google's Project Suncatcher to Put ML Infrastructure in Space](https://blog.google/innovation-and-ai/models-and-research/google-research/google-project-suncatcher-facts/) ⭐️ 8.0/10

Google announced Project Suncatcher, a research moonshot to build space-based ML data centers consisting of solar-powered satellites carrying Google TPUs, networked via free-space optical inter-satellite links. The company published a preprint paper, "Towards a future space-based, highly scalable AI infrastructure system design," outlining progress on high-bandwidth satellite communication, orbital dynamics, and radiation effects on computing. The announcement signals that major tech companies are seriously exploring space as a way to escape Earth-bound constraints on AI compute, including energy supply, cooling, and land availability. If feasible, space-based AI infrastructure could reshape how hyperscalers plan data center capacity and energy sourcing, though significant technical and economic hurdles remain. The proposed architecture uses fleets of solar-powered satellites in sun-synchronous orbit with free-space optical inter-satellite links for high-bandwidth communication. Key challenges include radiation effects on TPUs, orbital dynamics, and the economics of launching and maintaining hardware in space compared to terrestrial data centers.

hackernews · xnx · Sep 24, 13:53 · [Discussion](https://news.ycombinator.com/item?id=49830606)

**Background**: Space-based data centers are a proposed concept to build AI compute infrastructure in orbit using space-based solar power, offering unlimited solar energy and radiative cooling. The idea has historical roots in military space architectures like the 1980s Strategic Defense Initiative's Brilliant Pebbles and the modern Space Development Agency's Proliferated Warfighter Space Architecture. Google's Project Suncatcher is part of a growing trend that includes startups like Starcloud and Orbital, which are also pursuing orbital AI compute.

<details><summary>References</summary>
<ul>
<li><a href="https://research.google/blog/exploring-a-space-based-scalable-ai-infrastructure-system-design/">Exploring a space-based, scalable AI infrastructure system design</a></li>
<li><a href="https://arxiv.org/html/2511.19468v1">Towards a future space-based, highly scalable AI infrastructure system design</a></li>
<li><a href="https://en.wikipedia.org/wiki/Space-based_data_center">Space-based data center</a></li>

</ul>
</details>

**Discussion**: Commenters expressed skepticism about the physics and economics of space-based data centers, with some suggesting ulterior motives such as lower ping times or military applications. Others pointed to existing efforts like Starcloud's proof-of-concept and noted Alphabet's significant stake in SpaceX, while one commenter drew a historical parallel to the CIA's Glomar Explorer project, hinting at possible dual-use technology.

**Tags**: `#Google`, `#ML infrastructure`, `#space computing`, `#data centers`, `#industry news`

---

<a id="item-3"></a>
## [Apple Pulls Advanced Data Protection in the UK, Creating Two-Tier Encryption](https://macanorak.com/two-tier-encryption-in-the-uk/) ⭐️ 8.0/10

Apple has withdrawn its Advanced Data Protection (ADP) feature for UK users, reverting affected iCloud data categories such as iCloud Backup, Photos, Notes, and iCloud Drive from end-to-end encryption back to Standard Data Protection, where Apple holds the decryption keys. This creates a two-tier encryption system in which UK users lose end-to-end encryption for nine additional iCloud categories, while the 14 categories that are end-to-end encrypted by default (including iCloud Keychain and Health) remain protected. This is a significant privacy and encryption policy development because it shows how a government demand can effectively force a major platform to weaken security for an entire country rather than fight the order in court. It sets a precedent that could encourage other governments to seek similar concessions, and it affects every UK iCloud user who relied on ADP to protect sensitive data from Apple, hackers, or lawful requests. ADP is an optional setting that raises the number of end-to-end encrypted iCloud categories from 14 to 23, storing decryption keys offline on trusted devices; without it, the additional categories revert to Standard Data Protection, where Apple holds the keys and can respond to lawful legal process. The change was reportedly driven by a legal order under the UK's Investigatory Powers Act 2016, and the public disclosure of such orders is itself illegal, which limits what Apple can say.

hackernews · ReturnoftheHack · Sep 24, 10:39 · [Discussion](https://news.ycombinator.com/item?id=49828731)

**Background**: Advanced Data Protection for iCloud is Apple's highest level of cloud data security: when enabled, trusted devices retain sole access to the encryption keys for most iCloud data, so even Apple cannot read it. By default, iCloud uses Standard Data Protection, in which data is encrypted in transit and on Apple's servers but the keys are also stored on Apple's servers. The UK's Investigatory Powers Act 2016 allows the government to issue secret technical capability notices compelling companies to assist with lawful interception, and reports in February 2025 indicated Apple received such an order concerning iCloud backups.

<details><summary>References</summary>
<ul>
<li><a href="https://support.apple.com/guide/security/advanced-data-protection-for-icloud-sec973254c5f/web">Advanced Data Protection for iCloud - Apple Support</a></li>
<li><a href="https://en.wikipedia.org/wiki/Investigatory_Powers_Act_2016">Investigatory Powers Act 2016 - Wikipedia</a></li>
<li><a href="https://www.idownloadblog.com/2025/02/26/how-to-turn-on-advanced-data-protection-for-icloud/">Why and how to enable Advanced Data Protection for iCloud Should You Enable "Advanced Data Protection" for iCloud on ... Do you use “Advance Data Protection” option of iCloud? Why or ... How to use Advanced Data Protection for iCloud on iPhone How to Turn on Apple’s Advanced Data Protection — And Why It ...</a></li>

</ul>
</details>

**Discussion**: Commenters are sharply divided on Apple's decision: some argue Apple had the courage to resist government demands in 2015 but no longer does, pointing to mandatory age-confirmation and KYC screens as evidence of eroding principles. Others note technical nuances, such as the fact that UK users' end-to-end encryption secrets may still be exposed under common use cases, and some call for Apple to withdraw from the UK market or stop selling to UK government entities. A recurring concern is that secret government orders effectively outlaw end-to-end encryption without public debate.

**Tags**: `#encryption`, `#privacy`, `#Apple`, `#UK policy`, `#iCloud security`

---

<a id="item-4"></a>
## [Liquid AI's LFM2.5-VL-DSpark Speeds Up Vision-Language Models](https://huggingface.co/blog/LiquidAI/lfm2-5-vl-dspark) ⭐️ 7.0/10

Liquid AI released LFM2.5-VL-DSpark, an experimental speculative decoding draft model for its LFM2.5-VL-3B vision-language model, adding 280M parameters (an 8.9% size increase) while delivering decode speedups of up to 3.13x on-device (Apple M5 Max with MLX) and 2.66x on H100 GPUs. The drafter is available on Hugging Face with support in llama.cpp, SGLang, and MLX-VLM. This matters because vision-language models are computationally intensive, and speculative decoding offers a way to accelerate inference without retraining or changing output quality, making multimodal AI more practical for edge and on-device deployments. The support across llama.cpp, SGLang, and MLX-VLM means practitioners can readily integrate it into existing pipelines. The drafter is a standalone sidecar with 4 attention layers, a Markov head, a confidence head, and block size 9; token embeddings and the LM head are shared from the target model at load time, so it must be paired with an LFM2.5-VL-3B-GGUF target file. End-to-end gains reach up to 2.62x on M5 Max and 2.27x on H100, though the approach has limits for vision workloads on edge hardware.

rss · Hugging Face Blog · Sep 24, 14:08

**Background**: Vision-language models (VLMs) are multimodal generative models that take images and text as input and produce text output, but they are computationally expensive, especially due to long visual token sequences. Speculative decoding is a technique that uses a smaller draft model to propose multiple tokens, which are then verified by the larger target model in parallel, speeding up generation without altering the final output. LFM2.5-VL-3B is Liquid AI's compact 3-billion-parameter VLM designed for efficient inference.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/blog/LiquidAI/lfm2-5-vl-dspark">Accelerating vision-language models with LFM2.5-VL-DSpark</a></li>
<li><a href="https://huggingface.co/LiquidAI/LFM2.5-VL-3B-DSpark-GGUF">LiquidAI/LFM2.5-VL-3B-DSpark-GGUF · Hugging Face</a></li>
<li><a href="https://www.liquid.ai/blog/lfm2-5-vl-dspark">LFM2.5-VL-DSpark: Accelerating vision-language models on edge ...</a></li>

</ul>
</details>

**Tags**: `#vision-language models`, `#model acceleration`, `#multimodal AI`, `#Hugging Face`, `#efficient inference`

---