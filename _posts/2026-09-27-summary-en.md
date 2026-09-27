---
layout: default
title: "Horizon Summary: 2026-09-27 (EN)"
date: 2026-09-27
lang: en
---

> From 25 items, 3 important content pieces were selected

---

1. [DeepSeek Unveils DSec Sandbox Platform Scaling to 380,000 Concurrent Sandboxes](#item-1) ⭐️ 8.0/10
2. [Reladraw: A Declarative Diagram Language With Manual Placement Control](#item-2) ⭐️ 7.0/10
3. [Drawgent: A Coding Agent That Works on a Live Excalidraw Canvas](#item-3) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [DeepSeek Unveils DSec Sandbox Platform Scaling to 380,000 Concurrent Sandboxes](https://arxiv.org/abs/2609.22978) ⭐️ 8.0/10

DeepSeek introduced DeepSeek Elastic Compute (DSec), a production sandbox platform that exposes FnCall, container, microVM, and full-VM backends through a unified SDK. The system reportedly supports 380,000 concurrent sandboxes across 160 EPYC-based server nodes, and the paper lists 131 authors. This is a significant scalability milestone for sandbox infrastructure, which is increasingly critical for large-scale agentic training and evaluation of LLMs. It positions DeepSeek alongside efforts like Google's ax, and the unusual author list has sparked discussion about talent-retention strategy in the AI industry. DSec unifies four sandbox backends—FnCall, container, microVM, and full-VM—under a single SDK, and the reported scale of 380,000 concurrent sandboxes on 160 nodes works out to roughly 2,375 sandboxes per node. The paper's author list is unusually long, with 31 additional authors not even shown on the page.

hackernews · shenli3514 · Sep 26, 18:22 · [Discussion](https://news.ycombinator.com/item?id=49859112)

**Background**: A sandbox is an isolated environment that runs untrusted or experimental code without affecting the host system, and it is widely used in cloud computing for security and multi-tenant isolation. Elastic compute platforms like Amazon EC2 and Alibaba Cloud ECS let users rent scalable virtual computing resources on demand. DSec applies these ideas to AI workloads, providing isolated execution environments for agentic LLM training and evaluation at very high density.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2609.22978">[2609.22978] DeepSeek Elastic Compute ( DSec ): A Sandbox...</a></li>
<li><a href="https://www.emergentmind.com/papers/2609.22978">DeepSeek Elastic Compute ( DSec ): A Sandbox Infrastructure for...</a></li>
<li><a href="https://wesearch.press/s/deepseek-elastic-compute-dsec-e21b1a15">DeepSeek Elastic Compute ( DSec ) · WeSearch</a></li>

</ul>
</details>

**Discussion**: Commenters were impressed by the scale—one called 380,000 concurrent sandboxes on 160 EPYC nodes "crazy stuff"—and noted similarities to Google's ax project. A recurring theme was the unusually large author list: some speculated it is a talent-retention or asset-protection strategy to keep competitors from identifying and poaching key contributors, while others joked that the more interesting story is how 131 authors coordinated to publish the paper.

**Tags**: `#DeepSeek`, `#elastic compute`, `#sandbox`, `#scalability`, `#distributed systems`

---

<a id="item-2"></a>
## [Reladraw: A Declarative Diagram Language With Manual Placement Control](https://github.com/reladraw/reladraw) ⭐️ 7.0/10

Reladraw is a new open-source diagram language that lets users specify where elements go while keeping a declarative syntax, aiming to serve both humans and AI agents. It ships with a browser playground, an npm install option, and a skill that can be used with Claude or other agents. Existing tools force a trade-off: auto-placement languages like Mermaid and Graphviz decide the layout for you, while manual tools like Draw.io are powerful but slow and hard for agents to manipulate. Reladraw targets the AI coding era, where diagrams are a high-bandwidth way to align a developer's mental model with an agent's output. Reladraw uses relative positioning rather than absolute coordinates, which early commenters found sufficient for most flowcharts, and it supports edge declarations with from/to directions. However, users reported bugs, such as a curved arrow not being rendered when an edge was declared from left to right, and some questioned the LLM-generated README.

hackernews · jpwalsh234 · Sep 26, 17:10 · [Discussion](https://news.ycombinator.com/item?id=49858513)

**Background**: Diagram-as-code tools let you define diagrams in text instead of dragging shapes in a GUI. Declarative languages such as Mermaid, Graphviz, and D2 automatically compute layout from the declared nodes and edges, which is convenient but removes fine-grained control over appearance. Reladraw tries to keep the text-based declarative workflow while giving the author explicit control over placement.

<details><summary>References</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=49858513">Show HN: Reladraw – A diagram language where you decide where ...</a></li>
<li><a href="https://github.com/reladraw/reladraw">reladraw/reladraw - GitHub</a></li>
<li><a href="https://blog.logrocket.com/complete-guide-declarative-diagramming-d2/">A complete guide to declarative diagramming with D2 GitHub - d2lang/d2: D2 is a modern diagram scripting language ... D2: A Modern Diagram-as-Code Language D2 Playground D2 Tour | D2 Documentation DECLARATIVE LANGUAGE HANDBOOK</a></li>

</ul>
</details>

**Discussion**: Commenters broadly validated the need, with one calling it "very needed in the AI coding age" and another noting Mermaid is bad for flowcharts where position matters. Skepticism centered on the LLM-generated README and minor bugs, while one user asked whether it could turn spoken architecture descriptions into diagrams.

**Tags**: `#diagramming`, `#developer-tools`, `#DSL`, `#AI-agents`, `#visualization`

---

<a id="item-3"></a>
## [Drawgent: A Coding Agent That Works on a Live Excalidraw Canvas](https://tangled.org/yanndegat.tngl.sh/drawgent) ⭐️ 7.0/10

Drawgent is a new tool that lets a coding agent operate directly on a live Excalidraw canvas, enabling visual collaboration with AI for diagramming and prototyping. It was shared on Tangled and quickly gained traction on Hacker News with 133 points and 35 comments. This reflects a broader trend of giving AI agents shared visual workspaces rather than text-only interfaces, which could change how developers brainstorm architectures and prototypes. It also highlights growing competition and experimentation around agent-friendly diagramming tools, including Excalidraw's own MCP server and Mermaid-based alternatives. The project is hosted at tangled.org/yanndegat.tngl.sh/drawgent and is tagged with AI agents, Excalidraw, diagramming, developer tools, and MCP. Community members noted that Excalidraw already offers its own first-party open source MCP endpoint and server, and one commenter open-sourced a similar project called whiteboard-agents for comparison.

hackernews · parasitid · Sep 26, 15:56 · [Discussion](https://news.ycombinator.com/item?id=49857729)

**Background**: Excalidraw is an open-source, web-based virtual whiteboard known for its hand-drawn visual style and real-time multi-user collaboration. The Model Context Protocol (MCP) is an open standard introduced by Anthropic in November 2024 to let AI systems like LLMs connect with external tools and data sources. A coding agent is an AI system that autonomously performs coding tasks such as writing, reviewing, and refactoring code. Drawgent combines these ideas by letting an agent manipulate a shared Excalidraw canvas.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Excalidraw">Excalidraw</a></li>
<li><a href="https://en.wikipedia.org/wiki/Model_Context_Protocol">Model Context Protocol - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/AI_coding_agent">AI coding agent</a></li>

</ul>
</details>

**Discussion**: Commenters were largely enthusiastic but also raised alternatives: one pointed to Excalidraw's own first-party MCP server, while another said they found Mermaid more agent-friendly and built an Obsidian plugin for it. A skeptic argued that the real value of diagramming comes from the human thinking process, and another developer shared a similar open-source project, whiteboard-agents, for comparison.

**Tags**: `#AI agents`, `#Excalidraw`, `#diagramming`, `#developer tools`, `#MCP`

---