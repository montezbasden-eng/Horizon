---
layout: default
title: "Horizon Summary: 2026-09-11 (EN)"
date: 2026-09-11
lang: en
---

> From 52 items, 9 important content pieces were selected

---

1. [Shopify abandons React Native for native Swift and Kotlin](#item-1) ⭐️ 8.0/10
2. [Mathematicians question whether OpenAI can be trusted with unpublished math](#item-2) ⭐️ 8.0/10
3. [OpenAI Launches Agents API to Host Agent Harnesses](#item-3) ⭐️ 8.0/10
4. [OpenAI Launches ChatGPT for Financial Services with GPT-6 Astra](#item-4) ⭐️ 8.0/10
5. [trynix.dev runs any Nix package in a browser VM](#item-5) ⭐️ 8.0/10
6. [Researcher uses Codex and ChatGPT to mine genomes for new antimicrobials](#item-6) ⭐️ 7.0/10
7. [OpenAI launches Data agent in ChatGPT Work](#item-7) ⭐️ 7.0/10
8. [OpenAI and GSA Expand Discounted AI Access for US Governments](#item-8) ⭐️ 7.0/10
9. [Datasette 1.0a39 and 0.65.4 security releases fix private table exposure](#item-9) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Shopify abandons React Native for native Swift and Kotlin](https://shopify.engineering/back-to-native) ⭐️ 8.0/10

Shopify announced on its engineering blog that it is migrating its mobile app away from React Native back to fully native Swift for iOS and Kotlin for Android. The reversal of a high-profile cross-platform bet has triggered a large debate on Hacker News (876 points, 595 comments) about cross-platform frameworks, team size, and AI-assisted migration. Shopify is one of the largest e-commerce platforms and a well-known React Native adopter, so its move back to native code is a significant case study that could influence how other companies weigh cross-platform frameworks against native development. The decision also fuels the ongoing industry debate over whether shared codebases actually reduce cost and complexity at scale. The migration involves rewriting the app in Swift and Kotlin, and community members report that AI coding assistants such as Codex and LLMs were used to inventory screens and scaffold native code, though some engineers argue the migration would have been feasible without LLMs. Shopify's engineering organization reportedly has around 3,000 engineers, a scale that critics cite as evidence of over-complication.

hackernews · fnthawar2 · Sep 10, 14:09 · [Discussion](https://news.ycombinator.com/item?id=49643982)

**Background**: React Native is an open-source UI framework created by Meta that lets developers build iOS and Android apps using JavaScript and React, sharing much of the codebase across platforms. Swift is Apple's native programming language for iOS and macOS, while Kotlin is JetBrains' language that Google has endorsed as the preferred language for Android development. Shopify had previously been a prominent advocate of React Native, making its reversal a notable signal in the long-running native-versus-cross-platform debate.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/React_Native">React Native</a></li>
<li><a href="https://en.wikipedia.org/wiki/Kotlin">Kotlin</a></li>

</ul>
</details>

**Discussion**: Commenters are sharply divided: some iOS engineers feel validated in their long-standing skepticism of shared codebases, while others argue the migration was feasible without LLMs and push back on the narrative that AI made it possible. A recurring theme is skepticism about Shopify's engineering scale, with one commenter comparing its 3,000 engineers to the ~60 engineers behind Chrome's 2008 launch and GTA 5's 150 credited software engineers.

**Tags**: `#react-native`, `#mobile-development`, `#ios`, `#android`, `#engineering-culture`

---

<a id="item-2"></a>
## [Mathematicians question whether OpenAI can be trusted with unpublished math](https://mathstodon.xyz/@andreasthom/117240535270608201) ⭐️ 8.0/10

Mathematician Andreas Thom publicly accused OpenAI of refusing to rule out that private ChatGPT conversations with researchers were used to train the models behind its September math breakthroughs, following a similar complaint by researcher Buckmaster. OpenAI reportedly replied that it "did not train on" the chats, but critics say the answer leaves open whether de-identified data influenced the models. The dispute strikes at the heart of research integrity and trust in proprietary AI tools, since mathematicians may now hesitate to share unpublished ideas with commercial models that could later claim credit for solving open problems. It also echoes broader debates over attribution and transparency in AI-assisted research, with figures like Terence Tao warning that such practices could disrupt mathematics' collaborative spirit. The allegations follow OpenAI's September announcements of math breakthroughs, including work on a non-sofic group whose proof was checked in Lean, and OpenAI's response only denies direct training on the chats without addressing whether de-identified data could have influenced the models. The case is complicated by the fact that researchers using tools like Codex on open problems are effectively feeding fresh training data into the system.

hackernews · pred_ · Sep 10, 06:49 · [Discussion](https://news.ycombinator.com/item?id=49639408)

**Background**: OpenAI has given many researchers free or paid access to its models, and internal systems are reportedly solving open mathematical problems at a surprising rate. Because large language models are trained on vast amounts of data, it can be difficult to determine whether a specific conversation influenced a model's later outputs. Attribution norms in mathematics normally require crediting prior work, so the question of whether private chats were used without acknowledgment raises serious ethical concerns.

<details><summary>References</summary>
<ul>
<li><a href="https://www.aichatdaily.com/ai-security/mathematicians-accuse-openai-using-unpublished-work-math-breakthroughs">Mathematicians accuse OpenAI of using unpublished work in ...</a></li>
<li><a href="https://pasqualepillitteri.it/en/news/15418/openai-said-never-touched-math-chats">After Buckmaster, Thom Too Accuses OpenAI of Using ...</a></li>
<li><a href="https://x.com/i/trending/2097877893548265873">Mathematicians Accuse OpenAI of Using Private ChatGPT Tal...</a></li>

</ul>
</details>

**Discussion**: Commenters on Hacker News were divided: some argued that if OpenAI were a human collaborator, publishing results from shared ideas without attribution would be clearly unethical, while others noted that both claims can be true—chats may improve model intuition while reinforcement learning on verifiable math independently discovers superhuman techniques. Several users also cautioned against demanding an immediate answer from OpenAI, pointing out that verifying which data-sharing knobs a user enabled is non-trivial and that the causal effect on outputs is unclear.

**Tags**: `#AI ethics`, `#OpenAI`, `#research integrity`, `#mathematics`, `#machine learning`

---

<a id="item-3"></a>
## [OpenAI Launches Agents API to Host Agent Harnesses](https://developers.openai.com/api/docs/guides/agents-api/overview) ⭐️ 8.0/10

OpenAI has launched the Agents API, which lets developers build production-ready agents in a single API call by specifying the task, model, tools, and environment, while OpenAI hosts and maintains the underlying Codex harness. The API is built around four concepts — Agent, Environment, Session, and Events/items — and includes automatic context compaction, multi-agent orchestration, programmatic tool calling, and MCP support. This marks a major AI vendor moving up the stack from raw model endpoints into the agent harness layer, potentially reshaping how agent products are built and where value accrues. It lowers the barrier for developers who lack the resources to build and operate their own harness, but raises concerns about vendor lock-in and the blurring line between LLM endpoints and agents. The API runs the Codex harness and manages agent infrastructure, with an optional sandbox or computer where agents access files, load skills, and run commands; developers can also opt to self-host their sandbox, which may ease switching between providers. Sessions are durable instances that work on tasks and respond to input, and the quickstart begins with an OpenAI-hosted sandbox.

hackernews · aquir · Sep 10, 19:43 · [Discussion](https://news.ycombinator.com/item?id=49649213)

**Background**: An agent harness (also called scaffolding) is the software infrastructure around a large language model that enables it to act as an agent — managing tool use, memory, state persistence, execution environments, and feedback loops, since the model itself is stateless and only produces text. The relationship is often summarized as Agent = Model + Harness, and popular harnesses include Anthropic's Claude Code, OpenAI's Codex, and Google DeepMind's Antigravity. Building a harness is a substantial engineering undertaking, which is why managed offerings like this API are attractive to developers.

<details><summary>References</summary>
<ul>
<li><a href="https://developers.openai.com/api/docs/guides/agents-api/overview">Agents API | OpenAI API</a></li>
<li><a href="https://openai.com/index/introducing-the-agents-api/">Introducing the Agents API | OpenAI</a></li>
<li><a href="https://en.wikipedia.org/wiki/Agent_harness">Agent harness</a></li>

</ul>
</details>

**Discussion**: Commenters broadly agree that the right abstraction for agents-as-a-product is still unsettled, with some noting that self-hosting the sandbox makes the offering more enticing and eases provider transitions. Others argue the distinction between LLM endpoints and agent harnesses will become meaningless, while one critic complains about vendor lock-in and demands access to the reasoning tokens they pay for.

**Tags**: `#OpenAI`, `#AI Agents`, `#API`, `#LLM`, `#Developer Tools`

---

<a id="item-4"></a>
## [OpenAI Launches ChatGPT for Financial Services with GPT-6 Astra](https://openai.com/index/introducing-chatgpt-financial-services) ⭐️ 8.0/10

OpenAI announced ChatGPT for Financial Services, a specialized offering that combines built-in financial datasets from providers like Daloopa, PitchBook, and LSEG News with the newly released GPT-6 Astra model. The product is designed for research, financial modeling, and producing client-ready materials. This marks OpenAI's first vertical-specific ChatGPT offering for the financial industry, potentially reshaping how banks, asset managers, and fintech firms handle research and compliance workflows. It also signals intensifying competition among AI vendors to bundle proprietary data with frontier models for enterprise adoption. The offering integrates datasets covering earnings transcripts, financial statements, company fundamentals, and private company information, and is powered by GPT-6 Astra, which OpenAI describes as its most capable model for hard end-to-end work. The announcement itself is brief and lacks pricing, availability, or technical benchmark details.

rss · OpenAI News · Sep 10, 07:00

**Background**: GPT-6 Astra is OpenAI's large language model released to approved users on September 3, 2026, with general availability the following day, and is positioned as state-of-the-art across computer use, coding, cybersecurity, and science. ChatGPT for Financial Services builds on this model by adding curated third-party financial data, addressing a common enterprise complaint that general-purpose chatbots lack reliable, up-to-date market information.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/introducing-chatgpt-financial-services/">Introducing ChatGPT for Financial Services | OpenAI</a></li>
<li><a href="https://en.wikipedia.org/wiki/GPT-6_Astra">GPT-6 Astra - Wikipedia</a></li>
<li><a href="https://openai.com/index/gpt-6-astra/">GPT-6 Astra: A new generation of intelligence | OpenAI</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#ChatGPT`, `#Financial Services`, `#GPT-6`, `#AI Applications`

---

<a id="item-5"></a>
## [trynix.dev runs any Nix package in a browser VM](https://simonwillison.net/2026/Sep/10/trynix/) ⭐️ 8.0/10

Farid Zakaria launched trynix.dev, a qemu-wasm powered x86_64 Linux virtual machine that runs entirely in the browser and can boot any Nix package from the past 13 years, addressable by URL such as https://trynix.dev/?pkg=python3%403.6.2. He also released trynix-preview, a GitHub Action that comments a link on a pull request so reviewers can boot that PR's build directly in the browser. This makes historical and reproducible software environments instantly shareable as plain URLs, removing the need for servers, containers, or local setup when inspecting a package or reviewing a pull request. It could meaningfully change how developers do code review and reproduce old environments, and it showcases how far browser-based virtualization with WebAssembly has come. The VM is an x86_64 Linux system emulated by qemu-wasm, which ports QEMU's TCG emulation to WebAssembly, so the guest runs entirely client-side with no backend servers. Packages are selected through a URL query parameter, and the past-13-year scope reflects the range of historical Nix package revisions that remain available and buildable.

rss · Simon Willison · Sep 10, 23:44

**Background**: Nix is a purely functional package manager, created in 2003 by Eelco Dolstra, that treats packages as immutable values and enables reproducible, declarative builds. WebAssembly is a portable binary instruction format for a stack-based virtual machine that runs in browsers and can call into JavaScript and Web APIs. QEMU is a widely used open-source machine emulator; qemu-wasm is an experimental port that lets QEMU's system emulation run inside a browser via WebAssembly.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/ktock/qemu-wasm">GitHub - ktock/qemu-wasm: QEMU on browser · GitHub</a></li>
<li><a href="https://en.wikipedia.org/wiki/Nix_(package_manager)">Nix (package manager)</a></li>
<li><a href="https://webassembly.org/">WebAssembly</a></li>

</ul>
</details>

**Tags**: `#nix`, `#webassembly`, `#qemu`, `#virtualization`, `#developer-tools`

---

<a id="item-6"></a>
## [Researcher uses Codex and ChatGPT to mine genomes for new antimicrobials](https://openai.com/index/using-codex-chatgpt-to-search-for-new-antimicrobials) ⭐️ 7.0/10

César de la Fuente's lab is using OpenAI's Codex and ChatGPT to search both living and extinct genomes for new antimicrobial candidates to combat drug-resistant infections, as detailed in an OpenAI case study. This illustrates a concrete real-world application of AI coding and language tools in scientific discovery, potentially accelerating the search for antibiotics at a time when antimicrobial resistance is a top global health threat. The case study is a promotional piece from OpenAI with limited technical depth, and no specific molecules, model versions, or validation results are disclosed in the summary.

rss · OpenAI News · Sep 10, 16:00

**Background**: Antimicrobial resistance (AMR) occurs when bacteria, viruses, fungi, and parasites evolve to withstand the drugs used to treat them, making infections harder to treat; the WHO estimates bacterial AMR was directly responsible for 1.27 million deaths in 2019. Genome mining is a bioinformatics approach that scans DNA sequences for genes or peptides with potential antimicrobial activity, and AI tools like Codex and ChatGPT can help automate and scale this search.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Antimicrobial_resistance">Antimicrobial resistance</a></li>
<li><a href="https://www.who.int/news-room/fact-sheets/detail/antimicrobial-resistance">Antimicrobial resistance</a></li>
<li><a href="https://link.springer.com/article/10.1007/s12602-026-11205-5">Integrated Genome Mining and Bioactivity-Guided Isolation of...</a></li>

</ul>
</details>

**Tags**: `#AI`, `#drug discovery`, `#antimicrobial resistance`, `#genomics`, `#OpenAI`

---

<a id="item-7"></a>
## [OpenAI launches Data agent in ChatGPT Work](https://openai.com/index/put-data-to-work) ⭐️ 7.0/10

OpenAI announced a Data agent within ChatGPT Work that lets users connect company data, uncover insights, and build interactive dashboards using natural language. Users add the Data Plugin in ChatGPT Work, connect their existing data sources and context, and start a conversation to investigate what changed. This signals a meaningful step in enterprise AI tooling, moving ChatGPT from a general assistant toward an intent-driven analytics layer that lets more employees answer data questions themselves. It could reshape how companies approach analytics stacks and reduce reliance on dedicated BI teams. The agent is accessed by adding the Data Plugin in ChatGPT Work, and it connects to the data sources and context users already have. OpenAI's announcement is brief and promotional, offering limited technical detail on supported data sources, governance, or pricing.

rss · OpenAI News · Sep 10, 15:00

**Background**: ChatGPT Work is OpenAI's enterprise-oriented offering that supports longer tasks such as creating slides, sheets, documents, and sites, along with Scheduled Tasks. The Data agent builds on this by adding natural-language access to company data and dashboard creation. Interest in agentic analytics has grown since OpenAI shared its internal data agent, with competitors like Claude plugins accelerating the space.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/put-data-to-work/">Now everyone can put data to work | OpenAI</a></li>
<li><a href="https://community.openai.com/t/introducing-the-data-agent-for-chatgpt-work/1396488">Introducing the Data Agent for ChatGPT Work - ChatGPT - OpenAI Developer Community</a></li>
<li><a href="https://promethium.ai/the-new-agentic-analytics-fabric-or-how-to-get-claude-to-talk-to-all-your-enterprise-data/">The New Agentic Analytics Fabric OR How to Get... - Promethium</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#ChatGPT`, `#Enterprise AI`, `#Data Analytics`, `#Natural Language Interface`

---

<a id="item-8"></a>
## [OpenAI and GSA Expand Discounted AI Access for US Governments](https://openai.com/index/expanding-ai-access-us-government) ⭐️ 7.0/10

OpenAI announced a partnership with the U.S. General Services Administration (GSA) to offer eligible federal, state, local, and tribal governments $0 license fees, 50% off usage, and expanded cyber defense support. Under the related OneGov agreement, federal agencies can purchase ChatGPT Enterprise for $1 per agency for one year starting in 2026. This significantly lowers the cost barrier for public sector AI adoption, potentially accelerating the deployment of generative AI across all levels of U.S. government. It also signals a deepening relationship between leading AI companies and government agencies, with implications for AI policy, procurement, and cybersecurity practices. The offer includes $0 license fees and 50% off usage for eligible government entities, plus expanded cyber defense support. The related OneGov deal prices ChatGPT Enterprise at $1 per federal agency for one year, a deeply discounted rate compared to standard enterprise pricing.

rss · OpenAI News · Sep 10, 07:00

**Background**: The General Services Administration (GSA) is the U.S. federal agency that manages government procurement and shared services, including the OneGov initiative that streamlines how agencies buy technology. ChatGPT Enterprise is OpenAI's business-focused version of its chatbot, offering enhanced security, privacy, and administrative controls. The Center for Internet Security has also launched an AI Cyber Defense Pilot using OpenAI's technology to help state and local organizations identify and prioritize cybersecurity findings.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/expanding-ai-access-us-government/">Expanding AI access and cyber defense for federal ... - OpenAI</a></li>
<li><a href="https://fedscoop.com/openai-chatgpt-enterprise-federal-government-gsa-deal-general-services-administration-anthropic/">Federal agencies can buy ChatGPT for $1 through GSA deal | FedScoop</a></li>
<li><a href="https://www.cisecurity.org/about-us/media/press-release/center-for-internet-security-launches-ai-cyber-defense-pilot-to-strengthen-state-and-local-government-cybersecurity">Center for Internet Security Launches AI Cyber Defense Pilot ...</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#government`, `#AI access`, `#cybersecurity`, `#public sector`

---

<a id="item-9"></a>
## [Datasette 1.0a39 and 0.65.4 security releases fix private table exposure](https://simonwillison.net/2026/Sep/11/datasette-security/) ⭐️ 7.0/10

Datasette released two security patch versions, 1.0a39 for the alpha series and 0.65.4 for the stable 0.65.x family, fixing subtle bugs that could expose private tables on public instances. The fixes followed an extensive audit using Claude Fable 5.1, GPT-5.6, and GPT-6 Astra, plus nearly a week of collaborative human review after issues were reported by Sevban Dönmez and Alex Garcia. Anyone running a public Datasette instance that mixes public and private tables should upgrade immediately, since the flaws could leak private data. The release also signals a shift toward incorporating frontier-model security audits into routine open-source development, a practice other maintainers may adopt. The vulnerabilities are described as very subtle and specifically affect instances that serve a mixture of public and private tables in the same database, with access controlled by the Datasette permissions system. The audit workflow split work between two humans, with one writing automated tests that highlighted an issue and the other implementing the fix, while coding agents ran different models.

rss · Simon Willison · Sep 11, 03:27

**Background**: Datasette is an open-source tool for exploring and publishing data, letting users turn datasets into interactive websites and APIs. Its permissions system allows a single instance to serve both public and private tables, which is exactly the configuration where these subtle bugs could leak private table information. Earlier in 2026, Datasette 1.0a38 and 0.65.3 fixed a related SQL injection issue affecting instances mixing public and private tables.

<details><summary>References</summary>
<ul>
<li><a href="https://datasette.io/">Datasette: An open source multi-tool for exploring and publishing data</a></li>
<li><a href="https://simonwillison.net/2026/Aug/6/datasette/">Release: datasette 1.0a38</a></li>
<li><a href="https://www.anthropic.com/claude-fable-and-mythos-5-1">Introducing Claude Fable 5.1 and Claude Mythos 5.1</a></li>

</ul>
</details>

**Tags**: `#datasette`, `#security`, `#open-source`, `#vulnerability`, `#release`

---