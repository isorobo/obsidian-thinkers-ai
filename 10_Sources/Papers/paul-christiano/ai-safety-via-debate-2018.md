---
type: source
title: AI safety via debate
authors:
- Geoffrey Irving
- Paul Christiano
- Dario Amodei
thinker:
- '[[20_People/paul-christiano/profile|Paul Christiano]]'
source_type: paper
venue: arXiv preprint
year: 2018
url: https://arxiv.org/abs/1805.00899
domain:
- alignment
- scalable-oversight
- safety
status: inbox
created: 2026-06-07
tags:
- debate
- scalable-oversight
- self-play
- openai
arxiv_id: '1805.00899'
doi: ''
canonical_url: https://arxiv.org/abs/1805.00899
local_attachment: ''
source_hash: ''
retrieved_by: wiki-thinker-researcher
retrieved_at: 2026-06-07
nlm_source_id: ''
nlm_skip: false
topic:
- topic/debate
- topic/scalable-oversight
- topic/alignment
subject:
- subject/paul-christiano
wiki_indexed: '2026-06-07T10:00:00Z'
wiki_hash: 20a4fcfdd81af081f1d7a0a71a530b4124af55709d708a3592a7a9b32028f073
wiki_role: wiki
---


# AI safety via debate

## Citation

Irving, Geoffrey, Paul Christiano, and Dario Amodei. "AI safety via debate". arXiv preprint, 2018. https://arxiv.org/abs/1805.00899.

## One-line summary

The paper proposes training agents through a zero-sum debate game judged by humans, arguing that debate lets limited judges supervise questions beyond their direct reach.

## Key claims

- Asking humans to judge agent behaviour fails when the task is too complicated for direct human judgement.
- Two agents play a zero-sum debate game, making short statements, after which a human judges which gave the most true and useful information.
- By analogy to complexity theory, debate with optimal play answers any question in PSPACE given polynomial-time judges, while direct judging reaches only NP.
- An initial MNIST experiment shows debate boosting a sparse classifier from 59.4% to 88.9% accuracy given 6 pixels.
- Whether debate scales depends on empirical facts about humans and tasks plus theoretical questions about alignment.

## Excerpts

> "To help address this concern, we propose training agents via self play on a zero sum debate game."
> ~ Abstract

> "In an analogy to complexity theory, debate with optimal play can answer any question in PSPACE given polynomial time judges (direct judging answers only NP questions)."
> ~ Abstract

> "We report results on an initial MNIST experiment where agents compete to convince a sparse classifier, boosting the classifier's accuracy from 59.4% to 88.9% given 6 pixels and from 48.2% to 85.2% given 4 pixels."
> ~ Abstract

## Reveals about tendency of thought

- Christiano reaches for complexity-theory framing to argue about alignment, reflecting his theoretical-computer-science training.
- Debate and amplification are sibling answers to the same problem: how a weak supervisor oversees a stronger system.
- The honest caution about scaling weaknesses recurs across his work; he prefers stating where a proposal might break.

## Related

- [[10_Sources/Papers/paul-christiano/iterated-amplification-2018|Supervising strong learners by amplifying weak experts (2018)]] - companion scalable-oversight proposal
- [[10_Sources/Papers/paul-christiano/rlhf-2017|Deep reinforcement learning from human preferences (2017)]] - foundational human-feedback method
- [[20_People/paul-christiano/profile|Paul Christiano]]
