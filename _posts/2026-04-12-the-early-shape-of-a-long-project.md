---
layout: post
title: The Early Shape of a Long Project
description: "A personal journey into rethinking CPU front-ends — and why I think it's time to look beyond instructions."
date: 2026-04-18
categories: [computer-architecture, microarchitecture]
tags: [cpu, front-end, branch-prediction, hardware-design, semantic-analysis]
# featured: true
thumbnail: assets/img/alessandro-erbetta-8oYPewvmhnY-unsplash.jpg
related_posts: true
---

{% include figure.liquid 
    path="assets/img/alessandro-erbetta-8oYPewvmhnY-unsplash.jpg" 
    title="The Horizon of Microarchitecture" 
    width="65%"
    class="img-fluid rounded z-depth-1 mx-auto d-block" 
    caption="The path ahead isn’t always clear — but it’s worth walking."
%}

## 🎓 A New Chapter

It’s been a few months since I finished my PhD — in September 2024, *cum laude*, and with a lot of relief and a little pride. I still remember the moment: walking out of the defense room, heart pounding, and seeing my mom waiting with the biggest smile — and a hug that said everything.

{% include figure.liquid 
    path="assets/img/me-and-mom-phd-day.jpeg" 
    title="The day I became Dr. Alexandre V. Jamet." 
    width="65%"
    class="img-fluid rounded z-depth-1 mx-auto d-block" 
    caption="My mom, my first supporter — and my proudest cheerleader."
%}

That moment wasn’t just about me. It was about all the late nights, the coffee-fueled coding sessions, the doubts, and the quiet encouragement that kept me going. And now? I’m ready to take that same energy — and curiosity — into something new.

I’d spent years deep in cache hierarchies, memory systems, and the usual suspects of high-performance computing. But I’ve always been drawn to the hard, the unexplored, the things that make you ask: *What if we did this differently?*

So I asked myself: What if I turned my attention to the front-end of a processor — the part that fetches and decodes instructions? It’s not the flashiest area. It’s often seen as a place of small, incremental improvements. But what if that’s exactly where a big shift could happen?

## 🤔 Why the Front-End?

For decades, the front-end — the fetch, decode, and branch prediction stages — has been based on the humble instruction as its base work unit. It’s where the CPU reads the code, but not where the *meaning* of the code is fully understood.

We’ve optimized branch prediction with **2-bit counters**, **global history tables**, and even **machine learning** — yet we still treat the instruction as a black box. A signal. A byte sequence.

But what if we stopped treating it that way?

What if we looked at the **semantic structure** of the program — the loops, the function calls, the control flow patterns — and used that to guide the front-end?

That’s the idea I’m starting to explore.


## 🔍 A Glimpse Into the Work Ahead

Over the next few months, I’ll be sharing some early thoughts and experiments — and yes, I know this is a long-term project. But I think it’s worth it.

Here’s what I’m thinking about:

1. **Semantic-Aware Branch Prediction** — Instead of just tracking history, what if we used program-level patterns — like loop boundaries or function call sites — to predict whether a branch will be taken?
2. **Semantic-Aware Branch Target Prediction** — Can we use the *context* of a branch — such as the function it’s in — to better predict where it will jump?
3. **Rethinking the Decode Stage** — What if we didn’t decode every instruction the same way? Could we skip or simplify decoding for predictable patterns?

These aren’t just ideas — they’re grounded in real data. I’ve already seen **up to a 12% reduction in Branch MPKI** on cloud workloads using non-ML approaches that leverage semantic insights. That’s not a small number — especially when you consider how much performance and energy is lost to mispredictions.

## 🧠 Why This Matters

Modern workloads — especially in the cloud — are becoming more complex. We have microservices, containers, serverless functions, and dynamic execution patterns. And yet, our CPUs are still built on assumptions from the 1990s.

We’re asking: *What if we could design front-ends that are not just faster, but smarter?*

Smarter in the sense that they understand the *intent* behind the code — not just the bits.

This isn’t about replacing ML — it’s about **complementing it**. Or even **replacing it** in some cases, where simplicity, predictability, and energy efficiency matter more than marginal gains.

## 🌱 A Long-Term Vision

I don’t expect to have all the answers by next month. But I do have a plan:

- Start with **small, focused experiments** — testing semantic features on real workloads.
- Build **prototypes** — not just simulations, but actual hardware-aware models.
- Share **early results** — even if they’re imperfect — because progress is more valuable than perfection.

And I’d love to have you along for the ride.

If you’ve ever wondered whether we’re designing CPUs the right way, or if there’s a better way to think about performance and energy, I’d love to have you along for the ride.

Stay tuned. 🚀