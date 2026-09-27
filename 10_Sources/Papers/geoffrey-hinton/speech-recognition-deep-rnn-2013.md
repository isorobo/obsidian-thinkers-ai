---
type: source
title: Speech Recognition with Deep Recurrent Neural Networks
authors:
- Alex Graves
- Abdel-rahman Mohamed
- Geoffrey Hinton
thinker:
- '[[20_People/geoffrey-hinton/profile|Geoffrey Hinton]]'
source_type: paper
venue: IEEE International Conference on Acoustics, Speech and Signal Processing (ICASSP)
year: 2013
url: https://arxiv.org/abs/1303.5778
domain:
- capability
status: inbox
created: 2026-08-17
tags:
- recurrent-neural-networks
- speech-recognition
- lstm
arxiv_id: '1303.5778'
doi: ''
canonical_url: https://arxiv.org/abs/1303.5778
local_attachment: ''
source_hash: ''
retrieved_by: wiki-thinker-researcher
retrieved_at: 2026-08-17
nlm_source_id: ''
nlm_skip: false
topic:
- topic/speech-recognition
- topic/training-dynamics
subject:
- subject/geoffrey-hinton
- subject/alex-graves
- subject/lstm
- subject/connectionist-temporal-classification
- subject/timit
wiki_indexed: '2026-08-17T08:20:52Z'
wiki_hash: 90537186afb057134a518023696d5d60bc17d8331832412785f67148a95deb22
wiki_role: wiki
---


# Speech Recognition with Deep Recurrent Neural Networks

## Citation

Graves, A., Mohamed, A. and Hinton, G. "Speech Recognition with Deep Recurrent Neural Networks". IEEE International Conference on Acoustics, Speech and Signal Processing, 2013, pp. 6645-6649. https://arxiv.org/abs/1303.5778.

## One-line summary

Graves, Mohamed, and Hinton combine deep and recurrent architectures with LSTM units to set a new record on the TIMIT phoneme recognition task.

## Key claims

- Recurrent neural networks form a powerful model for sequential data such as speech.
- End-to-end training methods, including Connectionist Temporal Classification, allow RNN training without a known input-output alignment.
- Combining multiple representational layers with the flexible long-range context of recurrent networks improves speech recognition.
- Deep Long Short-Term Memory RNNs, trained end-to-end with suitable regularisation, achieve a 17.7% test-set error rate on TIMIT.
- This result represented the best recorded score on the TIMIT phoneme recognition benchmark at time of publication.

## Excerpts

> "Recurrent neural networks (RNNs) are a powerful model for sequential data."
> ~ Abstract

> "End-to-end training methods such as Connectionist Temporal Classification make it possible to train RNNs for sequence labelling problems where the input-output alignment is unknown."
> ~ Abstract

## Reveals about tendency of thought

- Hinton pairs architectural depth with sequence-model flexibility, rather than treating them as competing choices.
- The paper shows his group's practice of chasing state-of-the-art benchmark numbers as a proof of concept for a broader architectural idea.
- The move from acoustic modelling with feedforward networks to recurrent networks shows steady architectural escalation within a single research programme.

## Related

- [[10_Sources/Papers/geoffrey-hinton/acoustic-modeling-2012|Deep Neural Networks for Acoustic Modeling in Speech Recognition]] - the feedforward precursor this recurrent architecture extends.
- [[10_Sources/Papers/geoffrey-hinton/layer-normalization-2016|Layer Normalization]] - a later technique for stabilising recurrent network training.
- [[20_People/geoffrey-hinton/profile|Geoffrey Hinton]]
