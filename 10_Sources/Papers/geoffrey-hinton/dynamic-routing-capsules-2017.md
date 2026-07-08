---
type: source
title: Dynamic Routing Between Capsules
authors:
- Sara Sabour
- Nicholas Frosst
- Geoffrey Hinton
thinker:
- '[[20_People/geoffrey-hinton/profile|Geoffrey Hinton]]'
source_type: paper
venue: arXiv
year: 2017
url: https://arxiv.org/abs/1710.09829
domain:
- capability
status: verified
created: 2026-06-07
tags:
- capsule-networks
- routing-by-agreement
- computer-vision
- mnist
arxiv_id: '1710.09829'
doi: ''
canonical_url: https://arxiv.org/abs/1710.09829
local_attachment: ''
source_hash: ''
retrieved_by: wiki-thinker-researcher
retrieved_at: 2026-06-07
nlm_source_id: ''
topic:
- topic/training-dynamics
subject:
- subject/geoffrey-hinton
- subject/capsule-networks
- subject/computer-vision
wiki_indexed: '2026-06-14T12:00:00Z'
wiki_hash: 0a117ff294de7bac3524d26b082d6bde626061e885eb3411590cf2f441660cba
wiki_role: raw
---



# Dynamic Routing Between Capsules (2017)

## Citation

Sabour, Sara, Nicholas Frosst, and Geoffrey Hinton. "Dynamic Routing Between Capsules". arXiv:1710.09829, 2017. https://arxiv.org/abs/1710.09829.

## One-line summary

The paper introduces capsules, groups of neurons whose activity vectors encode the pose of an entity, and a routing-by-agreement mechanism that achieves state-of-the-art results on MNIST and excels at separating overlapping digits.

## Key claims

- A capsule is a group of neurons whose activity vector represents the instantiation parameters of an entity such as an object or an object part.
- The length of the activity vector encodes the probability that the entity exists; the orientation encodes its instantiation parameters.
- Active capsules at one level predict, through transformation matrices, the instantiation parameters of higher-level capsules.
- When multiple predictions agree, a higher-level capsule becomes active.
- A discriminatively trained, multi-layer capsule system reaches state-of-the-art performance on MNIST.
- The system surpasses a convolutional net at recognising highly overlapping digits.

## Excerpts

> "A capsule is a group of neurons whose activity vector represents the instantiation parameters of a specific type of entity such as an object or an object part."
~ "Abstract", arXiv:1710.09829

> "We use the length of the activity vector to represent the probability that the entity exists and its orientation to represent the instantiation parameters."
~ "Abstract", arXiv:1710.09829

> "Active capsules at one level make predictions, via transformation matrices, for the instantiation parameters of higher-level capsules. When multiple predictions agree, a higher level capsule becomes active."
~ "Abstract", arXiv:1710.09829

> "We show that a discriminatively trained, multi-layer capsule system achieves state-of-the-art performance on MNIST and is considerably better than a convolutional net at recognizing highly overlapping digits."
~ "Abstract", arXiv:1710.09829

> "A lower-level capsule prefers to send its output to higher level capsules whose activity vectors have a big scalar product with the prediction coming from the lower-level capsule."
~ "Abstract", arXiv:1710.09829

## Reveals about tendency of thought

- Part-whole structure: capsules encode pose and hierarchy, showing Hinton's long pursuit of representations that mirror how people parse scenes into parts and wholes.
- Dissatisfaction with convolutional pooling: routing-by-agreement replaces max-pooling, reflecting his view that pooling discards spatial information the brain retains.
- Vectors over scalars: representing entities as activity vectors rather than scalar activations signals a preference for richer, structured units of computation.
- Continuity with capsule work: the paper extends a research line that culminates in the later GLOM proposal on part-whole hierarchies.

## Related

- [[20_People/geoffrey-hinton/profile|Geoffrey Hinton]]
- [[10_Sources/Papers/geoffrey-hinton/glom-part-whole-hierarchies-2021|How to represent part-whole hierarchies in a neural network]]
- [[10_Sources/Papers/geoffrey-hinton/imagenet-alexnet-2012|ImageNet Classification with Deep Convolutional Neural Networks]]
- [[20_People/yann-lecun/profile|Yann LeCun]]
