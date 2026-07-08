---
type: source
title: Variational Option Discovery Algorithms
authors:
- Joshua Achiam
- Harrison Edwards
- Dario Amodei
- Pieter Abbeel
thinker:
- '[[20_People/dario-amodei/profile|Dario Amodei]]'
source_type: paper
venue: arXiv
year: 2018
url: https://arxiv.org/abs/1807.10299
domain:
- capability
status: review
created: '2026-04-27'
tags:
- paper
- reinforcement-learning
- options
- variational-inference
- curriculum
local_pdf: 20_People/dario-amodei/papers/1807.10299v1.pdf
dario_role: co-author
topic:
- topic/reinforcement-learning
- topic/options-framework
subject:
- subject/joshua-achiam
- subject/dario-amodei
- subject/openai
- subject/valor
wiki_indexed: '2026-06-07T10:00:00Z'
wiki_hash: 820920f4dc6211b89661cb366143575dce35cec961f61ffb4e6a22729060c3f9
wiki_role: wiki
---


# Variational Option Discovery Algorithms (2018)

## Citation

Joshua Achiam, Harrison Edwards, Dario Amodei, & Pieter Abbeel (2018). *Variational Option Discovery Algorithms*. arXiv. https://arxiv.org/abs/1807.10299

## One-line summary

Introduces VALOR (Variational Autoencoding Learning of Options by Reinforcement) and a curriculum trick that lets a single RL agent acquire many distinct behaviour modes via variational option discovery.

## Key claims

- Variational option discovery is structurally equivalent to a variational autoencoder with policies as encoders and trajectory decoders.
- VALOR encodes context noise into trajectories and decodes contexts back from full trajectories to learn diverse skills without external rewards.
- A simple curriculum that grows the context set as decoder accuracy rises stabilises training and enables more options.
- Identifies fundamental limits on option discovery purely from variational objectives without task-specific signal.

## Excerpts

> We explore methods for option discovery based on variational inference and make two algorithmic contributions. First: we highlight a tight connection between variational option discovery methods and variational autoencoders, and introduce Variational Autoencoding Learning of Options by Reinforcement (VALOR), a new method derived from the connection. In VALOR, the policy encodes contexts from a noise distribution into trajectories, and the decoder recovers the contexts from the complete trajectories. Second: we propose a curriculum learning approach where the number of contexts seen by the agent increases whenever the agent’s perfor- mance is strong enough (as measured by the decoder) on the current set of contexts. We show that this simple trick stabilizes training for VALOR and prior variational option discovery methods, allowing a single agent to learn many more modes of behavior than it could with a ﬁxed context distribution. Finally, we investigate other topics related to variational option discovery, including fundamental limitations of the general approach and the applicability of learned options to downstream tasks.
> ~ Abstract

## Reveals about tendency of thought

Placeholder. The original note did not record a tendency-of-thought analysis. Dario Amodei's role on this source: co-author. Local PDF: `20_People/dario-amodei/papers/1807.10299v1.pdf`.

## Related

- [[20_People/dario-amodei/profile|Dario Amodei]]
