---
type: source
title: "Beyond the Pelican Test: Claude Opus 5 Renders the Lord of the Rings"
authors:
- Andrej Karpathy
thinker:
- '[[20_People/andrej-karpathy/profile|Andrej Karpathy]]'
source_type: thread
venue: X (formerly Twitter)
year: 2026
url: https://x.com/karpathy/status/2083749667410727319
domain:
- capability
status: inbox
created: 2026-08-13
tags:
- evaluations
- claude-opus
- benchmarks
- three-js
arxiv_id: ''
doi: ''
canonical_url: https://x.com/karpathy/status/2083749667410727319
local_attachment: ''
source_hash: ''
retrieved_by: wiki-thinker-researcher
retrieved_at: 2026-08-13
nlm_source_id: ''
nlm_skip: true
---

# Beyond the Pelican Test: Claude Opus 5 Renders the Lord of the Rings

## Citation

Karpathy, Andrej. "We're starting to leave the territory where you'd test an LLM by e.g. 'create an svg of pelican on a bicycle'". X (formerly Twitter), 2 August 2026. https://x.com/karpathy/status/2083749667410727319.

## One-line summary

Karpathy tests Claude Opus 5 by asking it to render the opening of The Lord of the Rings as an interactive Three.js scene, arguing the exercise supersedes older single-prompt capability tests.

## Key claims

- Karpathy argues that simple prompts, such as drawing a pelican on a bicycle, no longer probe the frontier of model capability.
- He gave Claude Opus 5 the opening paragraph of The Lord of the Rings, a token budget of one million (about $10), and asked for a Three.js rendering.
- The model worked for about two hours and produced roughly 5,500 lines of code that procedurally generated and animated a 3D scene.
- He judges the output imperfect because the model could review its own work only through screenshots, not live video.
- He treats the exercise as an informal capability check rather than a formal benchmark, and links a playable version at karpathy.ai/lotr-movie.

## Excerpts

> "We're starting to leave the territory where you'd test an LLM by e.g. 'create an svg of pelican on a bicycle'."
> ~ Original tweet, 2 August 2026

> "I was interested what Opus 5 would do if I gave it the first paragraph of the Lord of the Rings, a 1M token budget (~$10) and asked for three js render of it."
> ~ Original tweet, 2 August 2026

> "It's kind of janky but fun."
> ~ Original tweet, 2 August 2026

> "[The model had to] place and orchestrate various polygon assets in (x,y,z) coordinates and write code that animates it all."
> ~ Original tweet, 2 August 2026

## Reveals about tendency of thought

- Karpathy continues his practice of inventing informal, memorable capability probes, favouring intuitive demonstrations over formal evaluation suites, in the same lineage as "vibe coding" and the verifiability formula.
- He treats cost and wall-clock time as first-class capability metrics, citing the exact dollar figure and duration alongside the qualitative result.
- The self-critical framing, calling the output "janky", shows his habitual honesty about model limitations even while showcasing a capability jump, consistent with the jagged-intelligence framing from his Sequoia Ascent talk.

## Related

- [[10_Sources/Articles/andrej-karpathy/sequoia-ascent-2026-summary|Sequoia Ascent 2026 Summary (2026)]] - source of the jagged-intelligence and verifiability framework this test extends
- [[10_Sources/Articles/andrej-karpathy/verifiability-2025|Verifiability (2025)]] - prior capability-prediction framework
- [[20_People/andrej-karpathy/profile|Andrej Karpathy]]
