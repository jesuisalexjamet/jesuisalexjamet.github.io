---
layout: post
title: <b>Enhancing Instruction Prefetching via Cache and TLB Management</b> accepted at <b>ISCA 2026</b>.
date: 2026-04-17 05:17:00+0100
inline: false
related_posts: false
---

I am happy to announce that our research paper entitled "Enhancing Instruction Prefetching via Cache and TLB Management" has been accepted for publication at ISCA 2026! 🥳 

This work addresses the underutilized potential of state-of-the-art L1I prefetchers by revealing two key limitations: 
 1. address translation latency undermines L1I page-cross prefetching timeliness, and .
 2. prefetched code lines exhibit highly variable reuse behavior, with many being dead-on-arrival.

To overcome these challenges, we propose IP-CaT (Instruction Prefetch Centric Cache and TLB Management), the first microarchitectural scheme that jointly orchestrates TLB and cache management to amplify L1I prefetching benefits. IP-CaT comprises two synergistic components: 
 1. the Translation Prefetch Buffer (tPB), a small buffer that stores page table entries fetched by L1I page-cross prefetches to reduce address translation latency, and;
 2. the Trimodal Instruction Prefetch Replacement Policy (TIPRP), a decision-tree based L2 cache replacement policy that judiciously manages prefetched code lines by anticipating their reuse potential.

We demonstrate that IP-CaT delivers significant performance improvements when integrated with three state-of-the-art L1I prefetchers (EPI, Barça, FNL+MMA), achieving up to 8.3% geomean speedup. IP-CaT substantially outperforms the state-of-the-art TLB management policy (CHiRP), the leading instruction TLB prefetcher (Morrigan), and state-of-the-art code-aware and general-purpose cache replacement policies (Emissary, SHiP++, Mockingjay).

Looking forward to presenting this work at ISCA 2026!
