---
layout: default
title: "Horizon Summary: 2026-09-02 (EN)"
date: 2026-09-02
lang: en
---

> From 54 items, 8 important content pieces were selected

---

1. [Anthropic Releases Claude Fable 5.1 and Mythos 5.1](#item-1) ⭐️ 9.0/10
2. [Dan Luu Critiques Ed Zitron's AI Predictions](#item-2) ⭐️ 8.0/10
3. [Slotstream Runs 125B Qwen3 on 48GB Mac at 12 tok/s via SSD Streaming](#item-3) ⭐️ 8.0/10
4. [OpenAI Connects ChatGPT to EHR and Healthcare Data](#item-4) ⭐️ 8.0/10
5. [BenchMIRT: Auditing LLM Benchmarks Question by Question](#item-5) ⭐️ 8.0/10
6. [Python 3.15.0 Release Candidate 2 Announced](#item-6) ⭐️ 8.0/10
7. [OpenAI's Codex App Bundles LibreOffice and Other Tools](#item-7) ⭐️ 7.0/10
8. [OpenAI Unveils Astra, First Model at Critical Cyber Threshold](#item-8) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Anthropic Releases Claude Fable 5.1 and Mythos 5.1](https://www.anthropic.com/claude-fable-and-mythos-5-1) ⭐️ 9.0/10

Anthropic has released Claude Fable 5.1 and Claude Mythos 5.1, featuring enhanced writing style, improved science performance, and reduced cache read pricing from $1/M to $0.25/M. The models are now available on the platform, with Fable 5.1 being a public-facing Mythos-class model and Mythos 5.1 restricted to vetted users. This release is significant because it directly addresses community feedback on writing quality and makes the model more cost-effective for developers, potentially increasing adoption. The price cut on cache reads could pressure competitors and reshape LLM pricing dynamics. Fable 5.1 shows gains in agentic coding and long-running workflows, with internal benchmarks showing it solves more coding problems than Fable 5 or Opus 5. The cache read price reduction from $1/M to $0.25/M makes Fable 5.1's cache reads half the cost of Opus's, and the system card is available for technical review.

hackernews · denysvitali · Sep 1, 17:53 · [Discussion](https://news.ycombinator.com/item?id=49525378)

**Background**: Claude Fable 5.1 is part of Anthropic's Mythos tier, which includes restricted-access models like Claude Mythos 5.1, designed for vetted users in cybersecurity and life sciences. The models are based on the same underlying architecture, with Fable 5.1 having safeguards that route certain requests to less capable models. Prompt caching allows developers to reduce costs by reusing cached prefixes, with cache reads typically costing 10% of standard input price.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/claude-fable-and-mythos-5-1">Introducing Claude Fable 5 . 1 and Claude Mythos 5 . 1 \ Anthropic</a></li>
<li><a href="https://en.wikipedia.org/wiki/Claude_Fable_5">Claude Fable 5</a></li>
<li><a href="https://openrouter.ai/anthropic/claude-fable-5.1">Claude Fable 5 . 1 - API Pricing & Providers | OpenRouter</a></li>

</ul>
</details>

**Discussion**: Community sentiment is mixed: an Anthropic employee praises the writing style improvements, while some users criticize the lack of significant benchmark gains and the removal of thought traces. One user notes that the price reduction suggests weak adoption of the original Fable, and there is skepticism about the marketing strategy around Mythos.

**Tags**: `#AI`, `#Anthropic`, `#Claude`, `#LLM`, `#Machine Learning`

---

<a id="item-2"></a>
## [Dan Luu Critiques Ed Zitron's AI Predictions](https://danluu.com/zitron/) ⭐️ 8.0/10

Dan Luu published a detailed critique of Ed Zitron's AI skeptic predictions, arguing that many are vague, unsupported, or misinterpreted. The essay sparked a debate with 599 comments. This critique matters because Ed Zitron is a prominent AI skeptic whose predictions influence public perception of the tech industry. The analysis highlights the importance of rigorous evaluation of tech commentary, especially in a polarized AI debate. Luu points out that Zitron's numbers often don't connect to a coherent argument, citing examples like Facebook MAU decline being linked to Meta's financial problems. The critique focuses on Zitron's 2024-2025 predictions and their literal text.

hackernews · jatins · Sep 1, 18:35 · [Discussion](https://news.ycombinator.com/item?id=49526069)

**Background**: Ed Zitron is a tech commentator known for his skeptical views on AI, often discussing the 'rot economy' where products decline despite financial success. Dan Luu is a software engineer and blogger who frequently analyzes tech industry claims with data. This critique is part of a broader discourse on the validity of AI predictions.

**Discussion**: Commenters debated the interpretation of 'dying' in Zitron's predictions, with some arguing it refers to product quality decline rather than company failure. Others noted that people often project their own predictions onto Zitron's statements, moving away from his actual claims. Some agreed with Luu's point about numbers not supporting arguments, while others defended Zitron's media presence over accuracy.

**Tags**: `#AI`, `#criticism`, `#predictions`, `#tech industry`, `#analysis`

---

<a id="item-3"></a>
## [Slotstream Runs 125B Qwen3 on 48GB Mac at 12 tok/s via SSD Streaming](https://github.com/carloslfu/slotstream) ⭐️ 8.0/10

Slotstream, a new tool built with MLX and Swift, enables running the 125B-parameter Qwen3.8-Flash-Next 4-bit model on Macs with as little as 16GB unified memory, achieving ~12 tok/s on a 48GB Mac. It uses expert offloading and SSD streaming to keep memory usage low, and includes an auto-mode that balances memory and speed. This project demonstrates a practical way to run very large MoE models on consumer hardware, potentially lowering the barrier for local LLM inference. It aligns with a growing trend of SSD-streaming and expert-offloading techniques that extend the effective memory of devices without requiring expensive upgrades. The model is Qwen3.8-Flash-Next, a 125B-parameter MoE model, quantized to 4-bit. Slotstream is Mac-native, using Apple's MLX framework and Swift, and supports auto-mode for automatic memory-speed tradeoffs. The developer plans to implement and port the MTP module for speculative decoding next.

hackernews · carloslfu · Sep 1, 16:42 · [Discussion](https://news.ycombinator.com/item?id=49524447)

**Background**: Mixture-of-Experts (MoE) models contain many specialized sub-networks (experts), but only a few are active per token, allowing selective loading. Expert offloading and SSD streaming store inactive experts on disk and load them on demand, trading slower I/O for much lower memory usage. MLX is Apple's array framework for machine learning on Apple silicon, enabling efficient inference on Macs.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2411.01433">[2411.01433] HOBBIT: A Mixed Precision Expert Offloading ... Enable Expert Offloading - General - vLLM Forums GitHub - caiovicentino/vllm-expert-offload: A high-throughput ... fMoE: Fine-Grained Expert Offloading for Large Mixture-of ... Awesome MoE LLM Inference System and Algorithm SSD Offloading for LLM Mixture-of-Experts Weights Considered ... Two-Stage Expert Offloading for Domain-Aware MoE Inference</a></li>
<li><a href="https://github.com/tonbistudio/moe-ssd-streaming-windows">GitHub - tonbistudio/moe-ssd-streaming-windows: Running a 32 ... SSD Streaming for AI Models: How to Turn RAM from a Wall into ... GitHub - giannisanni/pulsar: SSD-streaming inference engine ... I built a Rust inference engine that streams MoE expert ... ds4: The SSD-Streaming Inference Engine That Treats Your Mac ... Streaming from SSD: when the model exceeds RAM SolidAttention: Low-Latency SSD-based Serving on Memory ...</a></li>
<li><a href="https://mlx-framework.org/">MLX</a></li>

</ul>
</details>

**Discussion**: Community comments show a mix of skepticism and optimism. Some users question the claimed speeds on 16GB machines, citing thermal and memory constraints, while others express hope that such techniques will make larger models usable on upcoming hardware like the 32GB M6. There are also suggestions for improving the README and discussions about adding more RAM to GPUs.

**Tags**: `#LLM`, `#MLX`, `#model inference`, `#memory optimization`, `#Mac`

---

<a id="item-4"></a>
## [OpenAI Connects ChatGPT to EHR and Healthcare Data](https://openai.com/index/chatgpt-connects-health-records-and-healthcare-sources) ⭐️ 8.0/10

OpenAI announced that ChatGPT for Healthcare can now integrate with Epic's electronic health record (EHR) system and a new Healthcare Public Data plugin, allowing clinicians to securely access authorized patient data and structured information from official sources. This integration supports workflows such as reviewing patient histories and preparing for appointments. This development is significant because it brings large language models into direct contact with sensitive patient data, potentially improving clinical workflows and patient care. It also raises important considerations for privacy and security, as healthcare organizations must ensure HIPAA compliance when using AI tools. The Epic integration supports two main workflows: pulling authorized patient data into ChatGPT for review, and using the Healthcare Public Data plugin to work with structured information from official sources. Epic's EHR system holds data for over 325 million patients, making this a broad-reaching integration.

rss · OpenAI News · Sep 1, 12:00

**Background**: Electronic health records (EHRs) are digital versions of patients' medical histories, and integrating AI with them can help clinicians quickly access relevant information. HIPAA (Health Insurance Portability and Accountability Act) sets standards for protecting sensitive patient data, and AI tools used in healthcare must comply with these regulations. OpenAI has previously introduced OpenAI for Healthcare, which supports HIPAA compliance, and this new integration builds on that foundation.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/chatgpt-connects-health-records-and-healthcare-sources/">Healthcare organizations can now connect EHR and additional ...</a></li>
<li><a href="https://www.fiercehealthcare.com/ai-and-machine-learning/chatgpt-healthcare-unveils-new-integrations-epic-ehr-public-health-data">ChatGPT for Healthcare unveils new integrations with Epic ...</a></li>
<li><a href="https://techcrunch.com/2026/09/01/chatgpt-health-adds-epic-integration-for-clinicians-to-import-patient-data/">ChatGPT Health adds Epic integration for clinicians to import ...</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Healthcare`, `#ChatGPT`, `#Data Integration`, `#Privacy`

---

<a id="item-5"></a>
## [BenchMIRT: Auditing LLM Benchmarks Question by Question](https://huggingface.co/blog/allenai/benchmirt) ⭐️ 8.0/10

BenchMIRT is a new method for auditing LLM benchmarks question by question, revealing which capabilities they actually measure and helping researchers build smaller, more focused, and easier-to-interpret evaluations. This matters because it addresses the growing concern about the validity of LLM benchmarks, which are widely used to compare models but may not measure what they claim. By improving benchmark validity, BenchMIRT could lead to more reliable model evaluations and better-informed decisions in the AI community. The method analyzes benchmarks at the individual question level to identify the signals they contain, potentially allowing for the removal of redundant questions and the creation of more efficient benchmarks. The blog post from AI2 on Hugging Face discusses what BenchMIRT reveals about existing benchmarks and what it could mean for LLM evaluation.

rss · Hugging Face Blog · Sep 1, 21:39

**Background**: LLM benchmarks are standardized tests used to evaluate and compare large language models, such as MMLU and Chatbot Arena. However, there is growing concern about their construct validity—whether they actually measure the capabilities they claim to measure. BenchMIRT aims to address this by providing a method to audit benchmarks question by question, helping researchers understand what each question truly tests.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/blog/allenai/benchmirt">BenchMIRT : What are LLM benchmarks actually measuring?</a></li>
<li><a href="https://arxiv.org/abs/2511.04703">[2511.04703] Measuring what Matters: Construct Validity in ... New Report: Expanding the AI Evaluation Toolbox with ... Measuring what Matters: Construct Validity in Large Language ... LLM Evaluation Framework - Open-Source Guide & Benchmarks BenchMIRT: What are LLM benchmarks actually measuring?</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#benchmarks`, `#evaluation`, `#AI/ML`, `#research`

---

<a id="item-6"></a>
## [Python 3.15.0 Release Candidate 2 Announced](https://simonwillison.net/2026/Sep/1/python-315-rc-2/) ⭐️ 8.0/10

Python 3.15.0 release candidate 2 (RC2) has been announced by release manager Hugo van Kemenade, marking the final release candidate before the stable release scheduled for October. Third-party maintainers are strongly encouraged to test and publish wheels for Python 3.15 on PyPI. This release candidate is critical for the Python ecosystem as it signals the final opportunity for third-party projects to ensure compatibility before the stable release. Early testing and wheel publication help prevent bugs and ensure a smooth transition for the entire community. During the release candidate phase, only clear bug fixes are allowed between RC2 and the final release. Binary wheels built against Python 3.15.0 release candidates will work with future versions of Python 3.15. The new RC is not yet available on GitHub Actions, but can be tested using actions/setup-python with allow-prereleases and check-latest flags.

rss · Simon Willison · Sep 1, 14:59

**Background**: Python releases follow a structured cycle, with release candidates (RCs) serving as the final preview before a stable release. During the RC phase, only bug fixes are allowed, and third-party maintainers are urged to test their packages and publish wheels to ensure compatibility. Wheels are pre-built binary packages that install faster and avoid compilation issues, especially for projects with C extensions.

<details><summary>References</summary>
<ul>
<li><a href="https://www.python.org/downloads/release/python-3150rc2/">Python Release Python 3.15.0rc2 | Python.org</a></li>
<li><a href="https://blog.python.org/2026/08/python-3150-rc1/">Python 3.15.0 candidate 1 is here! | Python Insider</a></li>
<li><a href="https://simonwillison.net/2026/Sep/1/python-315-rc-2/">Python 3.15.0 candidate 2 is here! - simonwillison.net</a></li>

</ul>
</details>

**Tags**: `#Python`, `#release`, `#software engineering`, `#ecosystem`

---

<a id="item-7"></a>
## [OpenAI's Codex App Bundles LibreOffice and Other Tools](https://simonwillison.net/2026/Sep/1/codex-libreoffice/) ⭐️ 7.0/10

Simon Willison discovered that OpenAI's Codex desktop app (now rebranded as ChatGPT) bundles a full Python installation, Node.js, Poppler, git, and the LibreOffice office suite in its ~/.cache/codex-runtimes/codex-primary-runtime folder, totaling 1.7GB. The app includes skills that tell Codex how to use these binaries for document handling. This discovery reveals how OpenAI is leveraging open-source tools to handle document processing within its AI desktop app, potentially improving its ability to read and manipulate files like old Excel spreadsheets. It also raises questions about the app's design choices and the implications of bundling large dependencies, which could affect user experience and disk usage. The bundled tools include LibreOffice headless (429.7 MB), Poppler (187.9 MB), git (148.1 MB), and libheif (4.7 MB), among others. The plugins folder contains skills that instruct Codex on how to locate and use these binaries for document-related tasks.

rss · Simon Willison · Sep 1, 19:03 · [Discussion](https://news.ycombinator.com/item?id=49527396)

**Background**: Codex is OpenAI's AI coding agent that can execute tasks on a user's machine. The desktop app bundles a runtime environment with various tools to enable local processing of documents and other files. LibreOffice is a free, open-source office suite that can handle a wide range of document formats, including older Microsoft Office files. Poppler is a PDF rendering library, and git is a version control system.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/OmniDiskSweeper">OmniDiskSweeper - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Poppler_(software)">Poppler ( software ) - Wikipedia</a></li>
<li><a href="https://github.com/openai/codex/issues/30711">Codex Desktop (Microsoft Store) cannot complete Primary ...</a></li>

</ul>
</details>

**Discussion**: Community comments express mixed reactions. Some users suggest OpenAI should donate to LibreOffice to improve support for MS Office features, while others note that bundling LibreOffice is a practical way to read old files. There is also skepticism about whether the app bundles these tools from the start or downloads them on demand, and criticism of the app's overall design and dependency bloat.

**Tags**: `#OpenAI`, `#Codex`, `#LibreOffice`, `#software-bundling`, `#desktop-apps`

---

<a id="item-8"></a>
## [OpenAI Unveils Astra, First Model at Critical Cyber Threshold](https://openai.com/index/path-to-astra/) ⭐️ 7.0/10

OpenAI announced Astra, a new AI model that it claims meets the Critical cybersecurity capability threshold under its Preparedness Framework, making it the first model designated at this level. Access to Astra's advanced cybersecurity features will initially be limited to a small group of alpha testers, with broader defensive access through the Daybreak Blue program. This marks a significant milestone in AI capabilities and safety, as Astra is the first model to be classified at the critical cyber threshold, requiring enhanced safeguards. The decision to restrict access to its most powerful cybersecurity features highlights the growing tension between enabling defensive use and mitigating potential misuse, with implications for governments, enterprises, and the broader AI ecosystem. Astra achieved a perfect score on ExploitBench, a benchmark for developing exploits from known vulnerabilities, and can autonomously find and exploit previously unknown security flaws across well-protected systems. OpenAI paused some internal work on Astra in August to incorporate stricter safeguards, and the model's release will be phased, starting with alpha testers before expanding through Daybreak Blue.

hackernews · OpenAI News · Sep 1, 20:20 · [Discussion](https://news.ycombinator.com/item?id=49527595)

**Background**: OpenAI's Preparedness Framework defines capability thresholds for models with potentially dangerous capabilities, such as cybersecurity and biology. The Critical cybersecurity threshold indicates a model that can find and exploit vulnerabilities in many well-protected systems without human guidance, necessitating stronger safeguards. This announcement follows a recent incident involving OpenAI and Hugging Face, which underscored the urgency of strengthening monitoring and containment measures for frontier models.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/path-to-astra/">Path to Astra: critical capabilities and frontier safeguards | OpenAI</a></li>
<li><a href="https://www.bloomberg.com/news/articles/2026-09-01/openai-will-limit-access-to-new-astra-model-s-cybersecurity-features">OpenAI to Restrict Access to Astra AI Model’s Advanced Cybersecurity Tools - Bloomberg</a></li>
<li><a href="https://openai.com/index/responding-next-frontier-critical-cyber-capabilities/">Responding to the next frontier of critical cyber capabilities | OpenAI</a></li>

</ul>
</details>

**Discussion**: Community comments express skepticism about OpenAI's safety claims and access policies. One user criticizes the company for arbitrarily restricting access based on country of origin, while another notes the irony of Astra's perfect ExploitBench score in light of the recent Hugging Face hack. Others question whether governments might compel OpenAI to release unguarded model weights for national security, and some argue that many of Astra's capabilities have been available with good harness engineering for a year.

**Tags**: `#AI`, `#OpenAI`, `#safety`, `#security`, `#frontier models`

---