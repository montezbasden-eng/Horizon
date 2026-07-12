---
layout: default
title: "Horizon Summary: 2026-07-12 (EN)"
date: 2026-07-12
lang: en
---

> From 31 items, 3 important content pieces were selected

---

1. [RISCBoy: Open-Source RISC-V Retro Handheld Console](#item-1) ⭐️ 8.0/10
2. [Simple Liquids Can Fracture Like Solids](#item-2) ⭐️ 8.0/10
3. [Early History of the Singular Value Decomposition](#item-3) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [RISCBoy: Open-Source RISC-V Retro Handheld Console](https://github.com/Wren6991/RISCBoy) ⭐️ 8.0/10

Luke Wren, an ASIC design engineer at Raspberry Pi, has released RISCBoy, an open-source portable games console built from scratch around a RISC-V CPU and an FPGA. This project showcases a novel integration of the open RISC-V architecture in a retro gaming context, demonstrating that open-source hardware can replicate and innovate upon classic handheld designs without proprietary IP. RISCBoy is described as a 'Gameboy Advance from a parallel universe where RISC-V existed in 2001,' and its design includes open-source AHB/APB bus implementations, which are typically ARM-proprietary.

hackernews · mariuz · Jul 11, 21:58 · [Discussion](https://news.ycombinator.com/item?id=48876245)

**Background**: RISC-V is a free and open instruction set architecture (ISA) that allows anyone to design processors without paying royalties. FPGAs (field-programmable gate arrays) are configurable integrated circuits that can be reprogrammed after manufacturing, making them ideal for prototyping custom hardware like RISCBoy.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/RISC-V_Foundation">RISC-V Foundation</a></li>
<li><a href="https://en.wikipedia.org/wiki/FPGA">FPGA</a></li>

</ul>
</details>

**Discussion**: The community expressed admiration for Luke Wren's engineering skills, noting his previous work on DVI/HDMI from the RP2040. Some commenters were surprised that open-source AHB/APB implementations are permissible, as they had assumed those bus protocols were ARM-proprietary.

**Tags**: `#RISC-V`, `#open-source hardware`, `#retro gaming`, `#embedded systems`, `#FPGA`

---

<a id="item-2"></a>
## [Simple Liquids Can Fracture Like Solids](https://www.quantamagazine.org/we-know-simple-fluids-can-flow-turns-out-some-can-fracture-20260710/) ⭐️ 8.0/10

Researchers have discovered that simple liquids, such as hydrocarbon blends, can exhibit solidlike fracture when subjected to rapid shear or extensional flow, contradicting the long-held assumption that all simple fluids flow without breaking. This finding challenges fundamental understanding of liquid behavior and may have implications for industries like oil and gas, where fluid fracture could affect extraction processes. It suggests that fracture is a universal property of all liquids, not just complex or elastic fluids. The study, published in Physical Review Letters, used high-viscosity hydrocarbon blend liquids where the loss modulus G'' is an order of magnitude greater than the storage modulus G'. The fracture occurred while the liquid remained in its liquid state, not as a result of solidification.

hackernews · Anon84 · Jul 12, 02:13 · [Discussion](https://news.ycombinator.com/item?id=48877668)

**Background**: Simple liquids, like water or oil, are traditionally thought to flow continuously under stress, while solids fracture. Rheology studies how materials deform and flow; complex fluids (e.g., polymer solutions) can show both behaviors, but simple liquids were not expected to fracture. This discovery shows that even simple liquids can break when deformed quickly enough.

<details><summary>References</summary>
<ul>
<li><a href="https://phys.org/news/2026-03-liquids-fracture-solids.html">Liquids can fracture like solids —researchers discover the breaking...</a></li>
<li><a href="https://journals.aps.org/prl/abstract/10.1103/t2vy-32wr">Unexpected Solidlike Fracture in Simple Liquids | Phys. Rev. Lett.</a></li>
<li><a href="https://bioengineer.org/drexel-researchers-find-that-liquids-have-a-breaking-point/">Drexel Researchers Find That Liquids Have a Breaking Point</a></li>

</ul>
</details>

**Discussion**: Commenters raised questions about the role of inertia and viscosity, with some suggesting the effect might be universal for all liquids under extreme conditions. Others expressed ethical concerns about the research being funded by Exxon Mobil, given the fossil fuel industry's environmental impact. A few noted that glass, though not a simple fluid, has long been known to fracture.

**Tags**: `#physics`, `#fluids`, `#rheology`, `#materials science`, `#research`

---

<a id="item-3"></a>
## [Early History of the Singular Value Decomposition](https://www.math.ucdavis.edu/~saito/courses/229A/stewart-svd.pdf) ⭐️ 8.0/10

A 1993 historical paper by Stewart traces the development of the singular value decomposition (SVD) from its 19th-century origins to its modern formulation. SVD is a fundamental tool in linear algebra with widespread applications in machine learning, data compression, and numerical computing; understanding its history provides insight into its mathematical significance. The paper is dedicated to Gene Golub on his 15th birthday (a leap-year joke, as Golub was born on February 29), honoring his contributions to practical SVD algorithms.

hackernews · wolfi1 · Jul 11, 15:26 · [Discussion](https://news.ycombinator.com/item?id=48872858)

**Background**: The singular value decomposition factorizes any matrix into three components: U, Σ, and Vᵀ, where Σ contains singular values. It generalizes eigenvalue decomposition to non-square matrices and is central to many numerical methods.

**Discussion**: Commenters highlight SVD's ubiquity in computer vision and machine learning, with one noting that modern AI code generators frequently output SVD implementations. Another explains that singular values are like generalized eigenvalues, analogous to RGB color codes for matrices.

**Tags**: `#linear algebra`, `#singular value decomposition`, `#numerical analysis`, `#history of mathematics`

---