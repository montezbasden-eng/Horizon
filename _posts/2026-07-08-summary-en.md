---
layout: default
title: "Horizon Summary: 2026-07-08 (EN)"
date: 2026-07-08
lang: en
---

> From 44 items, 5 important content pieces were selected

---

1. [Tenda Firmware Backdoor Grants Admin Access](#item-1) ⭐️ 9.0/10
2. [MIT SICP Video Lectures (1986) Still Gold](#item-2) ⭐️ 8.0/10
3. [EU Chat Control 1.0 & 2.0: Scanning Communications Explained](#item-3) ⭐️ 8.0/10
4. [sqlite-utils 4.0 Introduces Database Schema Migrations](#item-4) ⭐️ 8.0/10
5. [Hugging Face to SageMaker Studio in One Click](#item-5) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Tenda Firmware Backdoor Grants Admin Access](https://kb.cert.org/vuls/id/213560) ⭐️ 9.0/10

Multiple versions of Tenda firmware contain a hidden authentication backdoor (CVE-2026-11405) that bypasses username validation, allowing attackers to gain full administrative access to the web management interface. This vulnerability is critical because it affects widely-used Tenda routers, enabling unauthenticated remote attackers to take full control of devices, potentially leading to network compromise, data theft, or use in botnets. The backdoor password is "rzadmin" and the associated username is not validated, so any username works with that password. Affected models include FH1201, W15E, AC10, AC5, and AC6 series.

hackernews · miniBill · Jul 8, 00:08 · [Discussion](https://news.ycombinator.com/item?id=48825749)

**Background**: Tenda is a Chinese manufacturer of home and business networking devices such as routers and switches. Firmware backdoors are undocumented access mechanisms sometimes left by developers for debugging, but they pose severe security risks if discovered by attackers.

<details><summary>References</summary>
<ul>
<li><a href="https://kb.cert.org/vuls/id/213560">VU#213560 - Tenda firmware (multiple versions) contains hidden authentication backdoor</a></li>
<li><a href="https://thehackernews.com/2026/07/certcc-warns-of-hidden-admin-backdoor.html">CERT/CC Warns of Hidden Admin Backdoor in Tenda Router Firmware</a></li>
<li><a href="https://www.bleepingcomputer.com/news/security/hidden-backdoor-in-tenda-router-firmware-grants-admin-access/">Hidden backdoor in Tenda router firmware grants admin access</a></li>

</ul>
</details>

**Discussion**: Commenters expressed strong distrust of router manufacturers, with many advocating for open-source firmware like OpenWRT. Some noted that the backdoor password "rzadmin" was publicly known since 2022, and criticized the amateur nature of the backdoor.

**Tags**: `#security`, `#vulnerability`, `#IoT`, `#firmware`, `#backdoor`

---

<a id="item-2"></a>
## [MIT SICP Video Lectures (1986) Still Gold](https://ocw.mit.edu/courses/6-001-structure-and-interpretation-of-computer-programs-spring-2005/video_galleries/video-lectures/) ⭐️ 8.0/10

MIT has made available the original 1986 video lectures for the classic computer science course 6.001, Structure and Interpretation of Computer Programs, taught by Harold Abelson and Gerald Jay Sussman. These lectures remain highly relevant for learning fundamental programming concepts like recursion, abstraction, and modularity, and are widely recommended by the programming community. The lectures use MIT Scheme, but the community suggests using Racket with the sicp package as a modern alternative. The video quality is original 1986, though some commenters note the sound may have been cleaned up.

hackernews · gjvc · Jul 7, 23:57 · [Discussion](https://news.ycombinator.com/item?id=48825664)

**Background**: SICP is a foundational computer science textbook known as the "Wizard Book" in hacker culture. It teaches programming principles using Scheme, a dialect of Lisp, and emphasizes the idea that computer programs are expressions of mathematical functions.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Structure_and_Interpretation_of_Computer_Programs">Structure and Interpretation of Computer Programs - Wikipedia</a></li>
<li><a href="https://mitp-content-server.mit.edu/books/content/sectbyfn/books_pres_0/6515/sicp.zip/index.html">Welcome to the SICP Web Site</a></li>

</ul>
</details>

**Discussion**: The community is overwhelmingly positive, with users calling the lectures "awesome" and saying they "cannot recommend these enough." One user found the lectures better than the book alone, and another suggested using Racket with the sicp package for a modern setup.

**Tags**: `#SICP`, `#computer science education`, `#programming`, `#MIT`, `#video lectures`

---

<a id="item-3"></a>
## [EU Chat Control 1.0 & 2.0: Scanning Communications Explained](https://fightchatcontrol.eu/chat-control-overview) ⭐️ 8.0/10

The EU is advancing two proposals, Chat Control 1.0 and 2.0, which would require messaging providers to scan all user communications for child sexual abuse material, potentially undermining end-to-end encryption. These proposals could set a global precedent for mass surveillance of private communications, threatening encryption and privacy for billions of users while aiming to combat child abuse. Chat Control 1.0 allows voluntary bulk scanning by large US providers, while Chat Control 2.0 mandates scanning of encrypted messages via client-side scanning, effectively bypassing end-to-end encryption.

hackernews · gasull · Jul 7, 14:23 · [Discussion](https://news.ycombinator.com/item?id=48818311)

**Background**: End-to-end encryption ensures that only the sender and recipient can read messages, but client-side scanning would analyze messages on the device before encryption, creating a potential backdoor. The EU argues this is necessary to detect illegal content, but critics warn it undermines privacy and could be abused.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Chat_Control">Chat Control - Wikipedia</a></li>
<li><a href="https://www.patrick-breyer.de/en/posts/chat-control/">Chat Control: The EU's CSAM scanner proposal</a></li>
<li><a href="https://www.internetsociety.org/resources/doc/2020/fact-sheet-client-side-scanning/">Fact Sheet: Client-Side Scanning - Internet Society</a></li>

</ul>
</details>

**Discussion**: Commenters express strong opposition, arguing the proposals are overly broad and ineffective, with some noting that client-side scanning circumvents encryption and could be bypassed by sideloading open-source clients. Concerns are raised about the impact on innocent users, such as parents taking photos of their children.

**Tags**: `#privacy`, `#encryption`, `#surveillance`, `#EU law`, `#child safety`

---

<a id="item-4"></a>
## [sqlite-utils 4.0 Introduces Database Schema Migrations](https://simonwillison.net/2026/Jul/7/sqlite-utils-4/#atom-everything) ⭐️ 8.0/10

sqlite-utils 4.0, released on July 7, 2026, adds database schema migrations, nested transactions via a new db.atomic() method, and support for compound foreign keys. This is the first major version bump since 2020, addressing long-standing user requests for migration support and making sqlite-utils more suitable for production database workflows. Migrations are defined in Python files using the sqlite-utils library, leveraging the table.transform() method for enhanced alter table capabilities beyond SQLite's native ALTER TABLE. The release also includes breaking changes detailed in an upgrade guide.

rss · Simon Willison · Jul 7, 19:32

**Background**: sqlite-utils is a Python library and CLI tool for manipulating SQLite databases. Schema migrations allow developers to version-control database schema changes and apply them incrementally, which is critical for applications that evolve over time.

<details><summary>References</summary>
<ul>
<li><a href="https://simonwillison.net/2026/Jul/7/sqlite-utils-4/">sqlite-utils 4.0, now with database schema migrations</a></li>
<li><a href="https://github.com/simonw/sqlite-migrate">GitHub - simonw/sqlite-migrate: A simple database migration system for SQLite, based on sqlite-utils · GitHub</a></li>
<li><a href="https://github.com/simonw/sqlite-utils/issues/117">Support for compound (composite) foreign keys · Issue #117 · simonw/sqlite-utils</a></li>

</ul>
</details>

**Tags**: `#sqlite`, `#database`, `#python`, `#data engineering`, `#open source`

---

<a id="item-5"></a>
## [Hugging Face to SageMaker Studio in One Click](https://huggingface.co/blog/amazon/one-click-to-sagemaker-studio) ⭐️ 7.0/10

Hugging Face and AWS announced a deep-link integration that allows developers to deploy models from Hugging Face to Amazon SageMaker Studio with a single click. This integration significantly reduces the friction for ML practitioners to move from model discovery to experimentation and deployment, streamlining the MLOps workflow on AWS. The one-click action launches SageMaker Studio directly from a Hugging Face model page, enabling immediate experimentation without manual setup. It builds on existing SageMaker JumpStart capabilities for Hugging Face models.

rss · Hugging Face Blog · Jul 7, 21:15

**Background**: Amazon SageMaker Studio is a fully integrated development environment (IDE) for machine learning. Hugging Face is a popular platform for hosting and sharing pre-trained models. Previously, deploying a Hugging Face model to SageMaker required multiple steps; this integration automates the process.

<details><summary>References</summary>
<ul>
<li><a href="https://aws.amazon.com/blogs/machine-learning/from-hugging-face-to-amazon-sagemaker-studio-in-one-click-2/">From Hugging Face to Amazon SageMaker Studio in one click | Artificial Intelligence</a></li>
<li><a href="https://docs.aws.amazon.com/sagemaker/latest/dg/hugging-face.html">Resources for using Hugging Face with Amazon SageMaker AI - Amazon SageMaker AI</a></li>
<li><a href="https://huggingface.co/docs/sagemaker/en/tutorials/jumpstart/jumpstart-quickstart">Quickstart - Deploy Hugging Face Models with SageMaker Jumpstart · Hugging Face</a></li>

</ul>
</details>

**Tags**: `#Hugging Face`, `#Amazon SageMaker`, `#MLOps`, `#deployment`

---