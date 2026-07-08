---
type: source
title: How to represent part-whole hierarchies in a neural network
authors:
- Geoffrey Hinton
thinker:
- '[[20_People/geoffrey-hinton/profile|Geoffrey Hinton]]'
source_type: essay
venue: arXiv
year: 2021
url: https://arxiv.org/abs/2102.12627
domain:
- capability
status: verified
created: 2026-06-07
tags:
- glom
- part-whole-hierarchies
- representation
- position-paper
arxiv_id: '2102.12627'
doi: ''
canonical_url: https://arxiv.org/abs/2102.12627
local_attachment: ''
source_hash: ''
retrieved_by: wiki-thinker-researcher
retrieved_at: 2026-06-07
nlm_source_id: ''
topic:
- topic/representation-learning
subject:
- subject/geoffrey-hinton
- subject/glom
- subject/part-whole-hierarchies
wiki_indexed: '2026-06-14T12:00:00Z'
wiki_hash: 7418901d2b2d52f4f0a5058806c9ba635e57df91c679edb91b246dc45e95b83a
wiki_role: raw
---



# How to represent part-whole hierarchies in a neural network (2021)

## Citation

Hinton, Geoffrey. "How to represent part-whole hierarchies in a neural network". arXiv:2102.12627, 2021. https://arxiv.org/abs/2102.12627.

## One-line summary

This position paper presents a single idea, islands of identical vectors, that combines transformers, neural fields, contrastive learning, distillation, and capsules into an imaginary system called GLOM for parsing images into part-whole hierarchies.

## Key claims

- The paper deliberately describes no working system; it presents one idea about representation.
- The idea allows advances from several groups to be combined into an imaginary system called GLOM.
- GLOM integrates transformers, neural fields, contrastive representation learning, distillation, and capsules.
- The core mechanism is to use islands of identical vectors to represent the nodes in the parse tree.
- People parse visual scenes into part-whole hierarchies and model spatial relations as coordinate transformations between intrinsic frames.
- If GLOM works, it should improve the interpretability of transformer-like systems applied to vision or language.

## Excerpts

> "This paper does not describe a working system. Instead, it presents a single idea about representation which allows advances made by several different groups to be combined into an imaginary system called GLOM."
~ "Abstract", arXiv:2102.12627

> "GLOM answers the question: How can a neural network with a fixed architecture parse an image into a part-whole hierarchy which has a different structure for each image?"
~ "Abstract", arXiv:2102.12627

> "The idea is simply to use islands of identical vectors to represent the nodes in the parse tree."
~ "Abstract", arXiv:2102.12627

> "If GLOM can be made to work, it should significantly improve the interpretability of the representations produced by transformer-like systems when applied to vision or language."
~ "Abstract", arXiv:2102.12627

> "There is strong psychological evidence that people parse visual scenes into part-whole hierarchies and model the viewpoint-invariant spatial relationship between a part and a whole as the coordinate transformation between intrinsic coordinate frames that they assign to the part and the whole."
~ "1 Overview of the idea", arXiv:2102.12627

## Reveals about tendency of thought

- Idea over implementation: Hinton publishes a conceptual proposal without code, treating a clear idea as a contribution in its own right.
- Synthesis instinct: he frames GLOM as a unifier of five separate advances, showing a drive to integrate rather than compete.
- Psychological grounding: he anchors the architecture in how people parse scenes, his decades-long lodestar.
- Interpretability concern: he motivates the design partly by the wish to understand what transformer-like systems represent.

## Related

- [[20_People/geoffrey-hinton/profile|Geoffrey Hinton]]
- [[10_Sources/Papers/geoffrey-hinton/dynamic-routing-capsules-2017|Dynamic Routing Between Capsules]]
- [[10_Sources/Papers/geoffrey-hinton/forward-forward-algorithm-2022|The Forward-Forward Algorithm]]
- [[20_People/yann-lecun/profile|Yann LeCun]]
