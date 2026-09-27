---
type: source
title: Reducing the Dimensionality of Data with Neural Networks
authors:
- Geoffrey E. Hinton
- Ruslan R. Salakhutdinov
thinker:
- '[[20_People/geoffrey-hinton/profile|Geoffrey Hinton]]'
source_type: paper
venue: Science
year: 2006
url: https://www.science.org/doi/10.1126/science.1127647
domain:
- capability
status: inbox
created: 2026-08-17
tags:
- autoencoders
- dimensionality-reduction
- deep-learning
arxiv_id: ''
doi: 10.1126/science.1127647
canonical_url: https://www.science.org/doi/10.1126/science.1127647
local_attachment: ''
source_hash: ''
retrieved_by: wiki-thinker-researcher
retrieved_at: 2026-08-17
nlm_source_id: ''
nlm_skip: false
topic:
- topic/representation-learning
- topic/training-dynamics
subject:
- subject/geoffrey-hinton
- subject/ruslan-salakhutdinov
- subject/autoencoders
- subject/principal-components-analysis
wiki_indexed: '2026-08-17T08:20:52Z'
wiki_hash: 9e5b5e7f410ac6bf481723c3c59d5fe2229e7c94c06063728f94f0e537ad6a01
wiki_role: wiki
---


# Reducing the Dimensionality of Data with Neural Networks

## Citation

Hinton, G. E. and Salakhutdinov, R. R. "Reducing the Dimensionality of Data with Neural Networks". Science, 313(5786), 2006, pp. 504-507. https://www.science.org/doi/10.1126/science.1127647.

## One-line summary

Hinton and Salakhutdinov show that a properly initialised deep autoencoder learns low-dimensional codes that beat principal components analysis.

## Key claims

- High-dimensional data converts to low-dimensional codes by training a multilayer network with a small central layer to reconstruct its input.
- Gradient descent fine-tunes the weights of such autoencoder networks, but only works well when initial weights sit close to a good solution.
- The paper describes an effective weight-initialisation method that lets deep autoencoders learn codes unavailable to shallow methods.
- The resulting codes outperform principal components analysis as a dimensionality-reduction tool.
- Layer-by-layer pretraining, later reused across deep learning, first proves its value in this paper.

## Excerpts

> "High-dimensional data can be converted to low-dimensional codes by training a multilayer neural network with a small central layer to reconstruct high-dimensional input vectors."
> ~ Abstract

> "Gradient descent can be used for fine-tuning the weights in such 'autoencoder' networks, but this works well only if the initial weights are close to a good solution."
> ~ Abstract

> "We describe an effective way of initializing the weights that allows deep autoencoder networks to learn low-dimensional codes that work much better than principal components analysis as a tool to reduce the dimensionality of data."
> ~ Abstract

## Reveals about tendency of thought

- Hinton favours architectural and initialisation fixes over larger models as the route to better representations.
- The paper shows his long-standing preference for unsupervised, layer-by-layer pretraining before fine-tuning.
- It demonstrates his habit of pairing a theoretical claim with a direct empirical comparison against an established baseline.

## Related

- [[10_Sources/Papers/geoffrey-hinton/deep-belief-nets-2006|A fast learning algorithm for deep belief nets]] - the companion 2006 paper that introduces the pretraining procedure this autoencoder result depends on.
- [[10_Sources/Papers/geoffrey-hinton/dynamic-routing-capsules-2017|Dynamic Routing Between Capsules]] - later work on learned part-whole representations.
- [[20_People/geoffrey-hinton/profile|Geoffrey Hinton]]
