---
type: source
title: Fine-Tuning Language Models from Human Preferences
authors:
- Daniel M. Ziegler
- Nisan Stiennon
- Jeffrey Wu
- Tom B. Brown
- Alec Radford
- Dario Amodei
- Paul Christiano
- Geoffrey Irving
thinker:
- '[[20_People/paul-christiano/profile|Paul Christiano]]'
source_type: paper
venue: arXiv
year: 2019
url: https://arxiv.org/abs/1909.08593
domain:
- alignment
- capability
status: inbox
created: 2026-10-04
tags:
- rlhf
- reward-learning
- language-models
- human-preferences
arxiv_id: '1909.08593'
doi: ''
canonical_url: https://arxiv.org/abs/1909.08593
local_attachment: ''
source_hash: ''
retrieved_by: wiki-thinker-researcher
retrieved_at: 2026-10-04
nlm_source_id: ''
nlm_skip: false
topic:
- topic/rlhf
wiki_indexed: '2026-10-04T03:18:02Z'
wiki_hash: 7d02745d7bbad336be3167beed246b56284df8a9710dc6f1eb768ed0267309aa
---

# Fine-Tuning Language Models from Human Preferences (2019)

## Citation

Ziegler, D. M., Stiennon, N., Wu, J., Brown, T. B., Radford, A., Amodei, D., Christiano, P. and Irving, G. "Fine-Tuning Language Models from Human Preferences". arXiv, 18 September 2019. https://arxiv.org/abs/1909.08593.

## One-line summary

The paper applies reward learning from human comparisons to pretrained language models on stylistic continuation and summarisation, and notes that the summarisers may exploit labeller heuristics.

## Key claims

- Reward learning lets RL address tasks where reward is defined by human judgment.
- The authors argue that reward learning for language is key to making RL practical and safe.
- Stylistic continuation works with only 5,000 human comparisons.
- Summarisation models copy whole sentences and may exploit simple labeller heuristics.

## Excerpts

> "Reward learning enables the application of reinforcement learning (RL) to tasks where reward is defined by human judgment, building a model of reward by asking humans questions."
> ~ Abstract, opening sentence

> "we believe reward learning for language is a key to making RL practical and safe for real-world tasks."
> ~ Abstract

> "For stylistic continuation we achieve good results with only 5,000 comparisons evaluated by humans."
> ~ Abstract

> "For summarization, models trained with 60,000 comparisons copy whole sentences from the input but skip irrelevant preamble; this leads to reasonable ROUGE scores and very good performance according to our human labelers, but may be exploiting the fact that labelers rely on simple heuristics."
> ~ Abstract, closing sentence

## Reveals about tendency of thought

- Reads as an early step in moving the reward-modelling agenda from games to language.
- Suggests candour about failure modes, since the abstract itself flags possible exploitation of labeller heuristics.

## Related

- [[20_People/paul-christiano/profile|Paul Christiano]]
