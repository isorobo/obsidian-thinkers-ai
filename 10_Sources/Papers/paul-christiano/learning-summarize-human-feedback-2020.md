---
type: source
title: Learning to summarize from human feedback
authors:
- Nisan Stiennon
- Long Ouyang
- Jeff Wu
- Daniel M. Ziegler
- Ryan Lowe
- Chelsea Voss
- Alec Radford
- Dario Amodei
- Paul Christiano
thinker:
- '[[20_People/paul-christiano/profile|Paul Christiano]]'
source_type: paper
venue: NeurIPS 2020
year: 2020
url: https://arxiv.org/abs/2009.01325
domain:
- alignment
- capability
status: inbox
created: 2026-10-04
tags:
- rlhf
- reward-modelling
- summarisation
- human-feedback
arxiv_id: '2009.01325'
doi: ''
canonical_url: https://arxiv.org/abs/2009.01325
local_attachment: ''
source_hash: ''
retrieved_by: wiki-thinker-researcher
retrieved_at: 2026-10-04
nlm_source_id: ''
nlm_skip: false
topic:
- topic/rlhf
- topic/summarisation
wiki_indexed: '2026-10-04T03:18:02Z'
wiki_hash: f7d455c5bd27034e3d8daa0dcec0d1a18568e2bde024fe9b62ae40550b1cbbc8
---

# Learning to summarize from human feedback (2020)

## Citation

Stiennon, N., Ouyang, L., Wu, J., Ziegler, D. M., Lowe, R., Voss, C., Radford, A., Amodei, D. and Christiano, P. "Learning to summarize from human feedback". NeurIPS 2020, 2020. https://arxiv.org/abs/2009.01325.

## One-line summary

The authors train a reward model on human comparisons of summaries and optimise a policy against it, producing summaries that humans prefer to those from much larger supervised models.

## Key claims

- Training and evaluation are increasingly bottlenecked by the data and metrics used for a task.
- A reward model trained on human comparisons, then optimised, beats supervised fine-tuning and human reference summaries.
- The models transfer to CNN/DM news without news-specific fine-tuning.
- The reward model generalises to new datasets and beats optimising ROUGE according to humans.

## Excerpts

> "As language models become more powerful, training and evaluation are increasingly bottlenecked by the data and metrics used for a particular task."
> ~ Abstract, opening sentence

> "Our models significantly outperform both human reference summaries and much larger models fine-tuned with supervised learning alone."
> ~ Abstract

> "Our models also transfer to CNN/DM news articles, producing summaries nearly as good as the human reference without any news-specific fine-tuning."
> ~ Abstract

> "We establish that our reward model generalizes to new datasets, and that optimizing our reward model results in better summaries than optimizing ROUGE according to humans."
> ~ Abstract, closing sentence

## Reveals about tendency of thought

- Suggests a commitment to testing alignment ideas on real language-model tasks with human feedback loops.
- Reads as a view that the proxy metric is the weak point, so the fix is to learn the objective from people.

## Related

- [[20_People/paul-christiano/profile|Paul Christiano]]
