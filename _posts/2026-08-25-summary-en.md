---
layout: default
title: "Horizon Summary: 2026-08-25 (EN)"
date: 2026-08-25
lang: en
---

> From 50 items, 5 important content pieces were selected

---

1. [MS Paint and Photos Embed Invisible GUID Watermarks in AI Images](#item-1) ⭐️ 8.0/10
2. [Interactive Moon Visualization Showcases Future of Web Education](#item-2) ⭐️ 8.0/10
3. [San Francisco Rendered as Playable 3D Web Game](#item-3) ⭐️ 8.0/10
4. [OpenAI Launches GPT-5.6 in Kiro with Better Price-Performance](#item-4) ⭐️ 8.0/10
5. [Turning SQLite Databases into Executable Linux Binaries](#item-5) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [MS Paint and Photos Embed Invisible GUID Watermarks in AI Images](https://xusheng.dev/posts/reversing/mspaint_invisible_watermark/main/) ⭐️ 8.0/10

A researcher found that Microsoft Paint and Photos silently embed a server-issued GUID as an invisible watermark in AI-manipulated images, even when the AI processing is done locally on Copilot+ PCs. The watermark cannot be disabled by users and persists even if the C2PA manifest is stripped. This raises significant privacy and anonymity concerns because the invisible GUID can be linked to a user's Microsoft account, potentially allowing authorities or third parties to trace image authorship. It also highlights a lack of transparency in widely used consumer software, affecting millions of users who may unknowingly embed identifying information in their creations. The invisible watermark is embedded at the pixel level and remains even after removing the C2PA manifest. The researcher found no user-accessible opt-out for the invisible watermark, and it applies to AI-manipulated images, including those generated locally on Copilot+ PCs, though prompt moderation may still be remote.

hackernews · ComputerGuru · Aug 24, 15:28 · [Discussion](https://news.ycombinator.com/item?id=49421158)

**Background**: Invisible watermarking is a technique that embeds imperceptible information into digital media to track ownership or provenance. C2PA is a standard for content authenticity that adds a manifest to images, but this GUID watermark goes beyond that by altering pixel data. Microsoft has been integrating AI features into Paint and Photos, and this watermarking appears to be part of their AI content provenance efforts, though it lacks user transparency.

<details><summary>References</summary>
<ul>
<li><a href="https://byteiota.com/ms-paint-invisible-server-guid-watermark-ai-image/">MS Paint Embeds Invisible Server GUIDs in Every AI Image | byteiota</a></li>
<li><a href="https://xusheng.dev/posts/reversing/mspaint_invisible_watermark/main/">Microsoft Paint and Photos Embed Server-Issued GUIDs ... :: Xusheng Li</a></li>
<li><a href="https://www.theregister.com/ai-and-ml/2026/08/25/microsoft-ai-watermarks-in-paint-and-photos-are-linked-to-user-ids-researcher-finds/5292034">Microsoft AI watermarks in Paint and Photos are linked to user IDs, researcher finds</a></li>

</ul>
</details>

**Discussion**: Community comments express shock and concern, with some noting that the AI aspect is a red herring and the real issue is the secret addition of unique identifiers to every image, which could be used to subpoena user data from Microsoft. Others point out past instances of Microsoft's sloppy AI implementations and recommend avoiding Paint and other LLM-enabled apps. There is also a mention of a false positive trigger, suggesting potential reliability issues.

**Tags**: `#privacy`, `#watermarking`, `#Microsoft`, `#AI`, `#security`

---

<a id="item-2"></a>
## [Interactive Moon Visualization Showcases Future of Web Education](https://ciechanow.ski/moon/) ⭐️ 8.0/10

Bartosz Ciechanowski released 'Moon (2024)', an interactive web page that explores the Moon's phases, orbit, and related phenomena with highly detailed visualizations. The page demonstrates advanced web techniques and has received high community engagement. This work exemplifies the potential of interactive web content for education, making complex astronomical concepts intuitive and engaging. It sets a standard for future educational web pages, especially as AI-assisted development makes such interactive pages more common. The page uses HTML5, JavaScript, and the Canvas API, consistent with Ciechanowski's earlier works. It includes detailed simulations of lunar phases, orbit mechanics, and eclipses, with a high level of interactivity. The page has been praised for its depth and visual quality.

hackernews · simonebrunozzi · Aug 24, 22:06 · [Discussion](https://news.ycombinator.com/item?id=49426466)

**Background**: Bartosz Ciechanowski is known for creating interactive explanatory web pages that make complex topics accessible. His works, such as 'Cameras and Lenses' and 'Bicycles', have been widely praised for their educational value. This new page continues his tradition of using web technologies to visualize scientific concepts.

<details><summary>References</summary>
<ul>
<li><a href="https://grokipedia.com/page/Bartosz_Ciechanowski">Bartosz Ciechanowski — Grokipedia</a></li>
<li><a href="https://tech.stonecharioteer.com/posts/2020/til-cameras-lenses-interactive-explanation/">TIL: Interactive Cameras and Lenses Explanation by Bartosz Ciechanowski | Stonecharioteer on Tech</a></li>
<li><a href="https://ericholscher.com/blog/2025/jan/7/everything-bartosz-ciechanowski-makes/">Everything Bartosz Ciechanowski makes is gold — Eric Holscher</a></li>

</ul>
</details>

**Discussion**: Community comments express admiration for the detail and interactivity, with some noting the lack of a table of contents and questioning the absence of the upcoming lunar eclipse in the full moon depiction. One user highlights Ciechanowski's influence on the future of web design, while another discusses using his style for AI-generated visualizations.

**Tags**: `#interactive visualization`, `#web development`, `#astronomy`, `#education`, `#Bartosz Ciechanowski`

---

<a id="item-3"></a>
## [San Francisco Rendered as Playable 3D Web Game](https://sf.thijs.gg/) ⭐️ 8.0/10

A web-based game at sf.thijs.gg renders the entire city of San Francisco as a playable 3D environment, allowing users to drive around and collect coins. The project was shared on Twitter by developer cdngdev, sparking significant community interest. This project demonstrates a novel approach to rendering real-world cities as interactive game environments using web technologies, which could inspire new applications in game development, urban planning, and virtual tourism. It also highlights the potential of using existing map data sources like Apple Maps for creating immersive experiences. The game appears to use retroplasma's reverse-engineered code for Apple's map data, though the community notes that retroplasma is outdated and incompatible with Apple's current data serving and HEIF texture format. The game runs entirely in a web browser, and the developer has hinted at potential future features like street names and address-based teleportation.

hackernews · centrosphere · Aug 24, 17:05 · [Discussion](https://news.ycombinator.com/item?id=49422784)

**Background**: Rendering real cities as 3D environments typically requires specialized software and data processing. This project leverages Apple's map data, which includes building footprints and elevation, to create a playable city. Web technologies like WebGL enable real-time 3D rendering in browsers, making such experiences accessible without downloads.

<details><summary>References</summary>
<ul>
<li><a href="https://www.tomshardware.com/tech-industry/ascii-cyberpunk-city-prototype-runs-on-rust-webassembly-engine-and-webgl-shaders">Walk through a 3 D cyberpunk city built purely from... | Tom's Hardware</a></li>
<li><a href="https://www.cgtrader.com/3d-models/san-francisco">San francisco 3D Models – Free & Premium Downloads | CGTrader</a></li>
<li><a href="https://makerworld.com/en/models/1200654-san-francisco-3d-map">San Francisco 3D Map - Free 3D Print Model - MakerWorld</a></li>

</ul>
</details>

**Discussion**: Community comments express excitement and emotional resonance, with one user who lived in SF for 20 years finding it moving. Technical discussions focus on the retroplasma pipeline and its limitations, while others suggest potential applications like generating GTA maps or creating an MMO. A user also shared a similar project for Philadelphia, indicating broader interest in this concept.

**Tags**: `#3D rendering`, `#game development`, `#map data`, `#San Francisco`, `#web technology`

---

<a id="item-4"></a>
## [OpenAI Launches GPT-5.6 in Kiro with Better Price-Performance](https://openai.com/index/gpt-5-6-in-kiro) ⭐️ 8.0/10

OpenAI has announced that GPT-5.6 is now available in Kiro, an agentic IDE, offering developers improved price-performance for planning, building, reviewing, and testing software. The model delivers more useful work per token, with stronger performance per dollar and on-demand capability for complex tasks. This release is significant because it directly addresses the cost concerns of developers using AI coding assistants, potentially accelerating adoption of agentic development tools. The improved price-performance could shift competitive dynamics among AI model providers, especially with the ongoing price war in the industry. The pricing for GPT-5.6 variants includes gpt-5.6-sol at $4.00 input and $20.00 output per 1M tokens, gpt-5.6-terra at $2.00 input and $12.00 output, and gpt-5.6-luna at $0.20 input and $1.20 output. These prices represent a 20% discount on input and 33% on output through at least November 21, 2026.

rss · OpenAI News · Aug 24, 12:00

**Background**: Kiro is an agentic IDE and command-line interface that helps developers go from prototype to production with spec-driven development, agent hooks, and natural language coding assistance. It was introduced by AWS and is designed to think like a developer, enabling autonomous, goal-driven actions. GPT-5.6 is OpenAI's latest model, and its integration into Kiro aims to provide a more cost-effective solution for AI-assisted software development.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/gpt-5-6-in-kiro/">Advancing price - performance for developers with GPT ‑ 5 . 6 in... | OpenAI</a></li>
<li><a href="https://github.com/kirodotdev/Kiro">GitHub - kirodotdev/Kiro: Kiro is an agentic IDE that works alongside you from prototype to production. · GitHub</a></li>
<li><a href="https://artificialanalysis.ai/models/gpt-5-6-sol">GPT - 5 . 6 Sol (max) - Intelligence, Performance & Price Analysis</a></li>

</ul>
</details>

**Discussion**: Community comments express mixed sentiments: some praise the price war and open-source models, while others note the significant discounts and compare pricing with Anthropic's offerings. One developer shares detailed opinions on when GPT-5.6 Sol fails compared to Fable, highlighting its focus on small details and struggles with longer multi-step tasks. Another user requests live price visualization on Artificial Analysis to better compare subscription costs.

**Tags**: `#AI`, `#OpenAI`, `#GPT-5.6`, `#Developer Tools`, `#Price-Performance`

---

<a id="item-5"></a>
## [Turning SQLite Databases into Executable Linux Binaries](https://simonwillison.net/2026/Aug/24/your-executable-is-a-sqlite-database/) ⭐️ 8.0/10

Farid Zakaria has developed a technique that allows a SQLite database file to be executed directly as a Linux binary by embedding ELF components into SQLite tables and using a custom interpreter called self-exec. The method leverages the SQLite application ID field and the Linux kernel's binfmt_misc mechanism to recognize and run such files. This innovation opens up new possibilities for software packaging and distribution, allowing a single file to serve both as a database and an executable. It could simplify deployment and enable creative use cases where data and code are tightly integrated, potentially influencing how developers approach application distribution on Linux. The technique sets the SQLite file's 4-byte application ID (at offset 68) to 'SELF' and arranges ELF components into multiple SQLite tables using a specific schema. The self-exec interpreter, written in C, extracts and executes the necessary parts, and binfmt_misc registration can be done via a simple printf command to /proc/sys/fs/binfmt_misc/register.

rss · Simon Willison · Aug 24, 11:38

**Background**: SQLite is a widely used embedded database that stores data in a single file, and its file format includes an application ID field for identifying the application that created it. ELF (Executable and Linkable Format) is the standard binary format for executables on Linux, containing headers, sections, and segments. binfmt_misc is a Linux kernel feature that allows custom binary formats to be registered and executed by user-space interpreters.

<details><summary>References</summary>
<ul>
<li><a href="https://stackoverflow.com/questions/35557487/where-can-i-register-a-sqlite-application-id">registration - Where can I register a sqlite application ID? - Stack Overflow</a></li>
<li><a href="https://en.wikipedia.org/wiki/Executable_and_Linkable_Format">Executable and Linkable Format - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Binfmt_misc">binfmt _ misc - Wikipedia</a></li>

</ul>
</details>

**Discussion**: The Hacker News discussion (linked in the article) likely includes reactions from developers, with some expressing interest in the hack and others discussing potential security implications or alternative approaches. However, specific comments are not provided in the search results, so the sentiment cannot be summarized accurately.

**Tags**: `#SQLite`, `#ELF`, `#Linux`, `#executable`, `#binfmt_misc`

---