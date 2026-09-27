---
type: source
title: Layer Normalization
authors:
- Jimmy Lei Ba
- Jamie Ryan Kiros
- Geoffrey E. Hinton
thinker:
- '[[20_People/geoffrey-hinton/profile|Geoffrey Hinton]]'
source_type: paper
venue: NIPS 2016 Deep Learning Symposium
year: 2016
url: https://arxiv.org/abs/1607.06450
domain:
- capability
status: inbox
created: 2026-08-17
tags:
- normalization
- recurrent-neural-networks
- training-stability
arxiv_id: '1607.06450'
doi: ''
canonical_url: https://arxiv.org/abs/1607.06450
local_attachment: ''
source_hash: ''
retrieved_by: wiki-thinker-researcher
retrieved_at: 2026-08-17
nlm_source_id: ''
nlm_skip: false
topic:
- topic/training-dynamics
- topic/regularisation
subject:
- subject/geoffrey-hinton
- subject/jimmy-ba
- subject/layer-normalisation
- subject/batch-normalisation
wiki_indexed: '2026-08-17T08:20:52Z'
wiki_hash: 59d96ce83e1b6d2b022aa4fce2e99b507780464bd8d50202c56a46a5b9e7d499
wiki_role: wiki
---


# Layer Normalization

## Citation

Ba, J. L., Kiros, J. R. and Hinton, G. E. "Layer Normalization". NIPS 2016 Deep Learning Symposium, 2016. https://arxiv.org/abs/1607.06450.

## One-line summary

Ba, Kiros, and Hinton introduce layer normalisation, a batch-independent alternative to batch normalisation suited to recurrent networks.

## Key claims

- Training state-of-the-art deep neural networks is computationally expensive.
- Normalising neuron activities reduces training time.
- Layer normalisation computes mean and variance from all summed inputs to the neurons in a single layer, for one training case, rather than across a mini-batch.
- The computation stays identical at training and test time, unlike batch normalisation.
- Layer normalisation applies straightforwardly to recurrent neural networks and stabilises their hidden state dynamics.
- Empirical results show layer normalisation substantially reduces training time relative to previously published methods.

## Excerpts

> "Training state-of-the-art, deep neural networks is computationally expensive. One way to reduce the training time is to normalize the activities of the neurons."
> ~ Abstract

> "Unlike batch normalization, layer normalization performs exactly the same computation at training and test times."
> ~ Abstract

> "Layer normalization is very effective at stabilizing the hidden state dynamics in recurrent networks."
> ~ Abstract

## Reveals about tendency of thought

- Hinton keeps returning to normalisation as a lever on training dynamics, from early weight-initialisation work through to this paper.
- The focus on recurrent networks shows sustained interest in sequence models alongside his vision-focused output.
- The paper favours a batch-independent method, reflecting a preference for techniques that generalise across model types.

## Related

- [[10_Sources/Papers/geoffrey-hinton/dropout-2014|Improving neural networks by preventing co-adaptation of feature detectors]] - an earlier regularisation and training-stability innovation from the same lab.
- [[10_Sources/Papers/geoffrey-hinton/speech-recognition-deep-rnn-2013|Speech Recognition with Deep Recurrent Neural Networks]] - the recurrent architecture this normalisation method later stabilises.
- [[20_People/geoffrey-hinton/profile|Geoffrey Hinton]]
