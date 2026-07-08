---
type: source
title: A General Language Assistant as a Laboratory for Alignment
authors:
- Amanda Askell
- Yuntao Bai
- Anna Chen
- Dawn Drain
- Deep Ganguli
- Tom Henighan
- Andy Jones
- Nicholas Joseph
- Ben Mann
- Nova DasSarma
- Nelson Elhage
- Zac Hatfield-Dodds
- Danny Hernandez
- Jackson Kernion
- Kamal Ndousse
- Catherine Olsson
- Dario Amodei
- Tom Brown
- Jack Clark
- Sam McCandlish
- Chris Olah
- Jared Kaplan
thinker:
- '[[20_People/dario-amodei/profile|Dario Amodei]]'
- '[[20_People/amanda-askell/profile|Amanda Askell]]'
- '[[20_People/chris-olah/profile|Chris Olah]]'
source_type: paper
venue: arXiv
year: 2021
url: https://arxiv.org/abs/2112.00861
domain:
- alignment
- capability
status: review
created: '2026-04-27'
tags:
- paper
- anthropic-foundational
- hhh
- preference-modelling
- prompting
local_pdf: 20_People/dario-amodei/papers/2112.00861v3.pdf
dario_role: co-author
topic:
- topic/alignment
- topic/helpful-honest-harmless
subject:
- subject/amanda-askell
- subject/jared-kaplan
- subject/dario-amodei
- subject/anthropic
- subject/hhh-framework
wiki_indexed: '2026-06-07T10:00:00Z'
wiki_hash: 015c65884d213ea1c738b2cbf00b6dab5d846417edcb9960e756dbcf3aa9a672
wiki_role: wiki
---


# A General Language Assistant as a Laboratory for Alignment (2021)

## Citation

Amanda Askell et al. (2021). *A General Language Assistant as a Laboratory for Alignment*. arXiv. https://arxiv.org/abs/2112.00861

## One-line summary

Anthropic's foundational alignment paper introducing the helpful-honest-harmless framework, baselining preference modelling against imitation and binary discrimination across model scales, and prefacing later RLHF and Constitutional AI work.

## Key claims

- Modest prompting interventions yield alignment gains that increase with model size and generalise across evaluations without harming performance.
- Ranked preference modelling outperforms imitation learning and binary discrimination, with more favourable scaling.
- Preference-model pre-training improves sample efficiency at the human-feedback fine-tuning stage.
- Establishes the helpful-honest-harmless triad as the operational target of Anthropic alignment work.

## Excerpts

> Given the broad capabilities of large language models, it should be possible to work towards a general-purpose, text-based assistant that is aligned with human values, meaning that it is helpful, honest, and harmless. As an initial foray in this direction we study simple baseline techniques and evaluations, such as prompting. We ﬁnd that the beneﬁts from modest interventions increase with model size, generalize to a variety of alignment evaluations, and do not compromise the performance of large models. Next we investigate scaling trends for several training objectives relevant to alignment, comparing imitation learning, binary discrimination, and ranked preference modeling. We ﬁnd that ranked preference modeling performs much better than imitation learning, and often scales more favorably with model size. In contrast, binary discrimination typically performs and scales very similarly to imitation learning. Finally we study a ‘preference model pre-training’ stage of training, with the goal of improving sample efﬁciency when ﬁnetuning on human preferences. ∗Core Research Contributors †Core Infrastructure Contributors ‡Correspondence to: jared@anthropic.com Author contributions are listed at the end of the paper. arXiv:2112.00861v3 [cs.CL] 9 Dec 2021 === PAGE BREAK === Contents
> ~ Abstract

## Reveals about tendency of thought

Placeholder. The original note did not record a tendency-of-thought analysis. Dario Amodei's role on this source: co-author. Local PDF: `20_People/dario-amodei/papers/2112.00861v3.pdf`.

## Related

- [[20_People/dario-amodei/profile|Dario Amodei]]
- [[20_People/amanda-askell/profile|Amanda Askell]]
- [[20_People/chris-olah/profile|Chris Olah]]
