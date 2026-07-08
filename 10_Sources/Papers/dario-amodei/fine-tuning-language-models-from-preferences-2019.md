---
type: source
title: Fine-Tuning Language Models from Human Preferences
authors:
- Daniel M Ziegler
- Nisan Stiennon
- Jeffrey Wu
- Tom B Brown
- Alec Radford
- Dario Amodei
- Paul Christiano
- Geoffrey Irving
thinker:
- '[[20_People/dario-amodei/profile|Dario Amodei]]'
- '[[20_People/paul-christiano/profile|Paul Christiano]]'
source_type: paper
venue: arXiv
year: 2019
url: https://arxiv.org/abs/1909.08593
domain:
- alignment
- capability
status: review
created: '2026-04-27'
tags:
- paper
- rlhf
- language-models
- sentiment-control
- summarisation
local_pdf: 20_People/dario-amodei/papers/1909.08593v2.pdf
dario_role: co-author
topic:
- topic/rlhf
- topic/language-model-finetuning
- topic/preference-learning
subject:
- subject/dario-amodei
- subject/paul-christiano
- subject/alec-radford
- subject/openai
- subject/gpt-2
wiki_indexed: '2026-06-07T10:00:00Z'
wiki_hash: eb788ee5a69d57bd6c1e2a06d8f2c102ba2d9e774c3bea45551693bda68af743
wiki_role: wiki
---


# Fine-Tuning Language Models from Human Preferences (2019)

## Citation

Daniel M Ziegler et al. (2019). *Fine-Tuning Language Models from Human Preferences*. arXiv. https://arxiv.org/abs/1909.08593

## One-line summary

First application of RLHF to natural-language tasks; fine-tunes GPT-style language models using preference feedback for sentiment continuation and summarisation, establishing the recipe behind ChatGPT-era systems.

## Key claims

- Reward learning generalises from RL control to natural-language generation by collecting preference comparisons over text continuations.
- 5,000 sentiment-style comparisons suffice to produce strong stylistic continuation; 60,000 summaries comparisons drive useful summarisation.
- Models exhibit reward-hacking on summarisation by copying input sentences whenever ROUGE rewards alignment with reference summaries.
- The pipeline directly anticipates the InstructGPT and ChatGPT training procedures.

## Excerpts

> Reward learning enables the application of rein- forcement learning (RL) to tasks where reward is deﬁned by human judgment, building a model of reward by asking humans questions. Most work on reward learning has used simulated environ- ments, but complex information about values is of- ten expressed in natural language, and we believe reward learning for language is a key to making RL practical and safe for real-world tasks. In this paper, we build on advances in generative pretrain- ing of language models to apply reward learning to four natural language tasks: continuing text with positive sentiment or physically descriptive language, and summarization tasks on the TL;DR and CNN/Daily Mail datasets. For stylistic con- tinuation we achieve good results with only 5,000 comparisons evaluated by humans. For summa- rization, models trained with 60,000 comparisons copy whole sentences from the input but skip irrel- evant preamble; this leads to reasonable ROUGE scores and very good performance according to our human labelers, but may be exploiting the fact that labelers rely on simple heuristics.
> ~ Abstract

## Reveals about tendency of thought

Placeholder. The original note did not record a tendency-of-thought analysis. Dario Amodei's role on this source: co-author. Local PDF: `20_People/dario-amodei/papers/1909.08593v2.pdf`.

## Related

- [[20_People/dario-amodei/profile|Dario Amodei]]
- [[20_People/paul-christiano/profile|Paul Christiano]]
