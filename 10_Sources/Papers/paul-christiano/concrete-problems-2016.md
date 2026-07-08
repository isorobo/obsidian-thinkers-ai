---
type: source
title: Concrete Problems in AI Safety
authors:
- Dario Amodei
- Chris Olah
- Jacob Steinhardt
- Paul Christiano
- John Schulman
- Dan Mané
thinker:
- '[[20_People/paul-christiano/profile|Paul Christiano]]'
source_type: paper
venue: arXiv preprint
year: 2016
url: https://arxiv.org/abs/1606.06565
domain:
- alignment
- safety
- machine-learning
status: inbox
created: 2026-06-07
tags:
- ai-safety
- reward-hacking
- safe-exploration
- accident-risk
arxiv_id: '1606.06565'
doi: ''
canonical_url: https://arxiv.org/abs/1606.06565
local_attachment: ''
source_hash: ''
retrieved_by: wiki-thinker-researcher
retrieved_at: 2026-06-07
nlm_source_id: ''
nlm_skip: false
topic:
- topic/ai-safety
- topic/alignment
subject:
- subject/paul-christiano
- subject/concrete-problems-in-ai-safety
wiki_indexed: '2026-06-07T10:00:00Z'
wiki_hash: 89b3e549c26c5811bf26a640466afcb55c54e2b4fb84a1822f324fc0a81ba5e5
wiki_role: wiki
---


# Concrete Problems in AI Safety

## Citation

Amodei, Dario, Chris Olah, Jacob Steinhardt, Paul Christiano, John Schulman, and Dan Mané. "Concrete Problems in AI Safety". arXiv preprint, 2016. https://arxiv.org/abs/1606.06565.

## One-line summary

The paper defines accident risk in machine learning and sets out five concrete, near-term safety research problems grounded in current systems.

## Key claims

- Accidents are unintended and harmful behaviours emerging from poor design of real-world AI systems.
- A wrong objective function produces two problems: avoiding side effects and avoiding reward hacking.
- An objective too expensive to evaluate frequently raises the scalable-supervision problem.
- Undesirable behaviour during learning splits into safe exploration and distributional shift.
- The five problems are practical, relevant to cutting-edge systems, and amenable to present-day research.

## Excerpts

> "In this paper we discuss one such potential impact: the problem of accidents in machine learning systems, defined as unintended and harmful behavior that may emerge from poor design of real-world AI systems."
> ~ Abstract

> "We present a list of five practical research problems related to accident risk, categorized according to whether the problem originates from having the wrong objective function ("avoiding side effects" and "avoiding reward hacking"), an objective function that is too expensive to evaluate frequently ("scalable supervision"), or undesirable behavior during the learning process ("safe exploration" and "distributional shift")."
> ~ Abstract

> "Finally, we consider the high-level question of how to think most productively about the safety of forward-looking applications of AI."
> ~ Abstract

## Reveals about tendency of thought

- Christiano co-authors the field's agenda-setting taxonomy, locating safety inside ordinary machine-learning practice rather than speculative scenarios.
- The "scalable supervision" problem named here becomes the spine of his later amplification and debate work.
- The roster of co-authors (Amodei, Olah, Schulman) maps the OpenAI safety circle he worked within.

## Related

- [[10_Sources/Papers/paul-christiano/rlhf-2017|Deep reinforcement learning from human preferences (2017)]] - addresses the wrong-objective problem through learned rewards
- [[10_Sources/Papers/paul-christiano/iterated-amplification-2018|Supervising strong learners by amplifying weak experts (2018)]] - attacks the scalable-supervision problem
- [[20_People/paul-christiano/profile|Paul Christiano]]
