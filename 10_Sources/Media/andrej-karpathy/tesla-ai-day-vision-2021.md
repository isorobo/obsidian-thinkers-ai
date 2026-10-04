---
type: source
title: Tesla AI Day - Andrej Karpathy on the Autopilot Vision Stack
authors:
- Elon Musk
- Andrej Karpathy
thinker:
- '[[20_People/andrej-karpathy/profile|Andrej Karpathy]]'
source_type: talk
venue: Tesla AI Day
year: 2021
url: https://elonmuskinterviews.wordpress.com/2021/08/31/tesla-ai-day-the-presentation-i/
domain:
- capability
- robotics
status: inbox
created: 2026-10-04
tags:
- tesla
- autopilot
- computer-vision
- self-driving
arxiv_id: ''
doi: ''
canonical_url: https://elonmuskinterviews.wordpress.com/2021/08/31/tesla-ai-day-the-presentation-i/
local_attachment: ''
source_hash: ''
retrieved_by: wiki-thinker-researcher
retrieved_at: 2026-10-04
nlm_source_id: ''
nlm_skip: false
topic:
- topic/computer-vision
wiki_indexed: '2026-10-04T03:18:02Z'
wiki_hash: f3eeda392cfbde87228ecb7631eb24f100ae2d9aa7e78a96a89557909ea7bd8e
---

# Tesla AI Day - Andrej Karpathy on the Autopilot Vision Stack (2021)

## Citation

Musk, E. and Karpathy, A. "Tesla AI Day - The Presentation (I)" (Karpathy's section on the vision stack). Tesla AI Day, 19 August 2021. https://elonmuskinterviews.wordpress.com/2021/08/31/tesla-ai-day-the-presentation-i/. Transcript via elonmuskinterviews.wordpress.com.

## One-line summary

Karpathy walks through how Tesla's Autopilot neural networks turn raw camera video into a vector-space representation of the driving scene, and how that architecture grew from single-image networks.

## Key claims

- The vision stack takes raw camera inputs and a neural net processes them into a vector space.
- Processing begins with the cameras, which Karpathy calls an artificial retina, then moves through feature fusion across scales into task-specific heads.
- The architecture grew far more complex than the simple single-image network of three or four years earlier.

## Excerpts

> "Hi, everyone. Welcome. My name is Andrej, and I lead the vision team here at Tesla autopilot."
> ~ Tesla AI Day, 19 August 2021, transcript position 48:35

> "Here I'm showing the video of the raw inputs that come into the stack, and then neural net processes that into the vector space."
> ~ Tesla AI Day, transcript position 49:47

> "So, the processing starts in the beginning when light hits our artificial retina."
> ~ Tesla AI Day, transcript position 51:13

> "After a BiFPN and a feature fusion across scales, we then go into task specific heads."
> ~ Tesla AI Day, transcript position 53:19

> "This architecture has definitely complexified from just a very simple image based single network about three or four years ago."
> ~ Tesla AI Day, transcript position 1:12:10

## Reveals about tendency of thought

- Reads as a systems-first view: the neural net is a pipeline from sensor to a unified vector-space world model.
- Suggests he treats progress as accumulated architectural complexity driven by real deployment needs rather than a single clean idea.

## Related

- [[10_Sources/Media/andrej-karpathy/cvpr-2021-tesla-autopilot|Tesla Autopilot at CVPR 2021]] - same team and stack, a few months earlier
- [[20_People/andrej-karpathy/profile|Andrej Karpathy]]
