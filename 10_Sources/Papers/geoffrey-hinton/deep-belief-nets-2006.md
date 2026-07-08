---
type: source
title: A fast learning algorithm for deep belief nets
authors:
- Geoffrey Hinton
- Simon Osindero
- Yee-Whye Teh
thinker:
- '[[20_People/geoffrey-hinton/profile|Geoffrey Hinton]]'
source_type: paper
venue: Neural Computation
year: 2006
url: https://pubmed.ncbi.nlm.nih.gov/16764513/
domain:
- capability
status: verified
created: 2026-06-07
tags:
- deep-belief-nets
- contrastive-divergence
- wake-sleep
- generative-models
arxiv_id: ''
doi: 10.1162/neco.2006.18.7.1527
canonical_url: https://pubmed.ncbi.nlm.nih.gov/16764513/
local_attachment: ''
source_hash: ''
retrieved_by: wiki-thinker-researcher
retrieved_at: 2026-06-07
nlm_source_id: ''
topic:
- topic/training-dynamics
subject:
- subject/geoffrey-hinton
- subject/deep-belief-nets
- subject/contrastive-divergence
wiki_indexed: '2026-06-14T12:00:00Z'
wiki_hash: 4326671a61fba648f5ca0747bdcc6a8da67600728fc2865242cddb8b6af41faa
wiki_role: raw
---



# A fast learning algorithm for deep belief nets (2006)

## Citation

Hinton, Geoffrey, Simon Osindero, and Yee-Whye Teh. "A fast learning algorithm for deep belief nets". Neural Computation 18, no. 7 (2006): 1527-1554. https://doi.org/10.1162/neco.2006.18.7.1527.

## One-line summary

The paper derives a fast, greedy, layer-by-layer learning procedure for deep belief networks that initialises a contrastive wake-sleep fine-tuning stage and builds a generative model beating discriminative methods on handwritten digits.

## Key claims

- Complementary priors eliminate the explaining-away effects that make inference hard in densely connected belief nets with many hidden layers.
- The fast, greedy algorithm learns deep, directed belief networks one layer at a time, provided the top two layers form an undirected associative memory.
- The greedy algorithm initialises a slower procedure that fine-tunes weights with a contrastive version of the wake-sleep algorithm.
- A network with three hidden layers becomes a strong generative model of the joint distribution of handwritten digit images and their labels.
- This generative model gives better digit classification than the best discriminative learning algorithms of the time.

## Excerpts

> "We show how to use 'complementary priors' to eliminate the explaining-away effects that make inference difficult in densely connected belief nets that have many hidden layers."
~ "Abstract", Neural Computation 18(7), 2006

> "Using complementary priors, we derive a fast, greedy algorithm that can learn deep, directed belief networks one layer at a time, provided the top two layers form an undirected associative memory."
~ "Abstract", Neural Computation 18(7), 2006

> "The fast, greedy algorithm is used to initialize a slower learning procedure that fine-tunes the weights using a contrastive version of the wake-sleep algorithm."
~ "Abstract", Neural Computation 18(7), 2006

> "After fine-tuning, a network with three hidden layers forms a very good generative model of the joint distribution of handwritten digit images and their labels. This generative model gives better digit classification than the best discriminative learning algorithms."
~ "Abstract", Neural Computation 18(7), 2006

## Reveals about tendency of thought

- Layer-wise learning: the greedy, one-layer-at-a-time procedure shows Hinton's instinct to decompose a hard global problem into tractable local steps.
- Generative-first stance: he prizes models of the joint distribution that beat discriminative methods, treating generation as the deeper test of understanding.
- Biological motifs: the wake-sleep algorithm and associative memory at the top echo his enduring effort to ground learning in brain-like mechanisms.
- Catalyst role: this 2006 result reopened deep network training and seeded the deep learning revival that followed.

## Related

- [[20_People/geoffrey-hinton/profile|Geoffrey Hinton]]
- [[10_Sources/Articles/geoffrey-hinton/rbm-practical-guide-2010|A Practical Guide to Training Restricted Boltzmann Machines]]
- [[10_Sources/Papers/geoffrey-hinton/imagenet-alexnet-2012|ImageNet Classification with Deep Convolutional Neural Networks]]
- [[20_People/yoshua-bengio/profile|Yoshua Bengio]]
