---
type: source
title: Deep Boltzmann Machines
authors:
- Ruslan Salakhutdinov
- Geoffrey Hinton
thinker:
- '[[20_People/geoffrey-hinton/profile|Geoffrey Hinton]]'
source_type: paper
venue: Proceedings of the Twelfth International Conference on Artificial Intelligence
  and Statistics (AISTATS)
year: 2009
url: https://proceedings.mlr.press/v5/salakhutdinov09a.html
domain:
- capability
status: inbox
created: 2026-08-17
tags:
- boltzmann-machines
- generative-models
- unsupervised-learning
arxiv_id: ''
doi: ''
canonical_url: https://proceedings.mlr.press/v5/salakhutdinov09a.html
local_attachment: ''
source_hash: ''
retrieved_by: wiki-thinker-researcher
retrieved_at: 2026-08-17
nlm_source_id: ''
nlm_skip: false
topic:
- topic/training-dynamics
- topic/representation-learning
subject:
- subject/geoffrey-hinton
- subject/ruslan-salakhutdinov
- subject/deep-boltzmann-machines
- subject/mnist
- subject/norb
wiki_indexed: '2026-08-17T08:20:52Z'
wiki_hash: f5acd9984809d4fcaea42c08d20ee5a20ec5fbaa049ea2f8892cd0b03194ab05
wiki_role: wiki
---


# Deep Boltzmann Machines

## Citation

Salakhutdinov, R. and Hinton, G. "Deep Boltzmann Machines". Proceedings of the Twelfth International Conference on Artificial Intelligence and Statistics, 5, 2009, pp. 448-455. https://proceedings.mlr.press/v5/salakhutdinov09a.html.

## One-line summary

Salakhutdinov and Hinton present a learning algorithm for multi-layer Boltzmann machines that scales to millions of parameters.

## Key claims

- The paper presents a new learning algorithm for Boltzmann machines containing many layers of hidden variables.
- Data-dependent expectations are estimated with a variational approximation that tends to focus on a single mode.
- Data-independent expectations are approximated using persistent Markov chains.
- Combining these two estimation techniques makes it practical to learn Boltzmann machines with multiple hidden layers and millions of parameters.
- A layer-by-layer pretraining phase initialises variational inference with a single bottom-up pass, improving learning efficiency.
- Results on MNIST and NORB show deep Boltzmann machines learn good generative models and perform well on digit and object recognition.

## Excerpts

> "We present a new learning algorithm for Boltzmann machines that contain many layers of hidden variables."
> ~ Abstract

> "The use of two quite different techniques for estimating the two types of expectation that enter into the gradient of the log-likelihood makes it practical to learn Boltzmann machines with multiple hidden layers and millions of parameters."
> ~ Abstract

> "We present results on the MNIST and NORB datasets showing that deep Boltzmann machines learn good generative models and perform well on handwritten digit and visual object recognition tasks."
> ~ Abstract

## Reveals about tendency of thought

- Hinton persists with generative, probabilistic models even as discriminative networks gain popularity elsewhere in the field.
- The paper's reuse of layer-by-layer pretraining across architectures shows a consistent methodological toolkit applied to new problems.
- Testing on both a digit dataset and an object dataset reflects his habit of demanding generality before declaring success.

## Related

- [[10_Sources/Papers/geoffrey-hinton/deep-belief-nets-2006|A fast learning algorithm for deep belief nets]] - the earlier layer-wise pretraining method this paper extends to fully undirected models.
- [[10_Sources/Papers/geoffrey-hinton/relu-rbm-2010|Rectified Linear Units Improve Restricted Boltzmann Machines]] - a unit-level improvement to the same family of models.
- [[20_People/geoffrey-hinton/profile|Geoffrey Hinton]]
