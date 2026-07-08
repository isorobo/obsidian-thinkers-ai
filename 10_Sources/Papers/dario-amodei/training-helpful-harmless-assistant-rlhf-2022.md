---
type: source
title: Training a Helpful and Harmless Assistant with Reinforcement Learning from
  Human Feedback
authors:
- Yuntao Bai
- Andy Jones
- Kamal Ndousse
- Amanda Askell
- Anna Chen
- Nova DasSarma
- Dawn Drain
- Stanislav Fort
- Deep Ganguli
- Tom Henighan
- Nicholas Joseph
- Saurav Kadavath
- Jackson Kernion
- Tom Conerly
- Sheer El Showk
- Nelson Elhage
- Zac Hatfield-Dodds
- Danny Hernandez
- Tristan Hume
- Scott Johnston
- Shauna Kravec
- Liane Lovitt
- Neel Nanda
- Catherine Olsson
- Dario Amodei
- Tom Brown
- Jack Clark
- Sam McCandlish
- Chris Olah
- Ben Mann
- Jared Kaplan
thinker:
- '[[20_People/dario-amodei/profile|Dario Amodei]]'
source_type: paper
venue: arXiv
year: 2022
url: https://arxiv.org/abs/2204.05862
domain:
- alignment
- capability
status: review
created: '2026-04-27'
tags:
- paper
- anthropic
- rlhf
- hhh
- online-learning
- kl-reward-tradeoff
local_pdf: 20_People/dario-amodei/papers/2204.05862v1.pdf
dario_role: co-author
topic:
- topic/rlhf
- topic/helpful-honest-harmless
- topic/alignment
subject:
- subject/yuntao-bai
- subject/jared-kaplan
- subject/dario-amodei
- subject/anthropic
- subject/claude-precursor
wiki_indexed: '2026-06-07T10:00:00Z'
wiki_hash: e772de035c99a4f6aa4b28a136a11d231ad2bbb3494d0548746f886351d55c28
wiki_role: wiki
---


# Training a Helpful and Harmless Assistant with Reinforcement Learning from Human Feedback (2022)

## Citation

Yuntao Bai et al. (2022). *Training a Helpful and Harmless Assistant with Reinforcement Learning from Human Feedback*. arXiv. https://arxiv.org/abs/2204.05862

## One-line summary

The canonical Anthropic RLHF paper that demonstrates iterated weekly online RLHF, identifies a square-root KL-reward scaling relation, and produces a helpful-harmless assistant whose training is the direct ancestor of Claude.

## Key claims

- RLHF on preference comparisons produces a helpful and harmless assistant compatible with downstream skill specialisation.
- Online iterated retraining on weekly fresh feedback efficiently improves both data and policy.
- RL reward versus square-root KL divergence between policy and base model exhibits a roughly linear relation, providing a tunable safety knob.
- The training stack is the immediate technical predecessor of Claude 1.

## Excerpts

> We apply preference modeling and reinforcement learning from human feedback (RLHF) to ﬁnetune language models to act as helpful and harmless assistants. We ﬁnd this align- ment training improves performance on almost all NLP evaluations, and is fully compatible with training for specialized skills such as python coding and summarization. We explore an iterated online mode of training, where preference models and RL policies are updated on a weekly cadence with fresh human feedback data, efﬁciently improving our datasets and models. Finally, we investigate the robustness of RLHF training, and identify a roughly linear relation between the RL reward and the square root of the KL divergence between the policy and its initialization. Alongside our main results, we perform peripheral analyses on calibration, competing objectives, and the use of OOD detection, compare our models with human writers, and provide samples from our models using prompts appearing in recent related work. ∗Correspondence to: {yuntao, jared}@anthropic.com Author contributions are listed at the end of the paper. arXiv:2204.05862v1 [cs.CL] 12 Apr 2022 === PAGE BREAK === Contents
> ~ Abstract

## Reveals about tendency of thought

Placeholder. The original note did not record a tendency-of-thought analysis. Dario Amodei's role on this source: co-author. Local PDF: `20_People/dario-amodei/papers/2204.05862v1.pdf`.

## Related

- [[20_People/dario-amodei/profile|Dario Amodei]]
