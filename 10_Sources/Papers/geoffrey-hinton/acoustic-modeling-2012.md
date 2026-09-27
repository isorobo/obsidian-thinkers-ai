---
type: source
title: 'Deep Neural Networks for Acoustic Modeling in Speech Recognition: The Shared
  Views of Four Research Groups'
authors:
- Geoffrey Hinton
- Li Deng
- Dong Yu
- George Dahl
- Abdel-rahman Mohamed
- Navdeep Jaitly
- Andrew Senior
- Vincent Vanhoucke
- Patrick Nguyen
- Tara Sainath
- Brian Kingsbury
thinker:
- '[[20_People/geoffrey-hinton/profile|Geoffrey Hinton]]'
source_type: paper
venue: IEEE Signal Processing Magazine
year: 2012
url: https://research.google/pubs/deep-neural-networks-for-acoustic-modeling-in-speech-recognition/
domain:
- capability
status: inbox
created: 2026-08-17
tags:
- speech-recognition
- deep-neural-networks
- acoustic-modeling
arxiv_id: ''
doi: 10.1109/msp.2012.2205597
canonical_url: https://research.google/pubs/deep-neural-networks-for-acoustic-modeling-in-speech-recognition/
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
- subject/microsoft
- subject/ibm
- subject/google-brain
wiki_indexed: '2026-08-17T08:20:52Z'
wiki_hash: 3096fd39ff29dc8687228429eb89ddd411c60058caeec3a88418abedfe21f1fd
wiki_role: wiki
---


# Deep Neural Networks for Acoustic Modeling in Speech Recognition

## Citation

Hinton, G., Deng, L., Yu, D., Dahl, G., Mohamed, A., Jaitly, N., Senior, A., Vanhoucke, V., Nguyen, P., Sainath, T. and Kingsbury, B. "Deep Neural Networks for Acoustic Modeling in Speech Recognition: The Shared Views of Four Research Groups". IEEE Signal Processing Magazine, 29, 2012. https://research.google/pubs/deep-neural-networks-for-acoustic-modeling-in-speech-recognition/.

## One-line summary

Hinton and eleven co-authors from four research groups summarise how deep neural networks overtook Gaussian mixture models in speech recognition.

## Key claims

- Speech recognition systems traditionally combine hidden Markov models with Gaussian mixture models to score acoustic frames.
- A feedforward neural network can replace the Gaussian mixture model, producing posterior probabilities over hidden Markov model states directly.
- Deep neural networks trained with new methods outperform Gaussian mixture models on multiple speech recognition benchmarks.
- The margin of improvement is large on some benchmarks, not merely incremental.
- The paper consolidates independent successes from four research groups into a shared account of the technique.

## Excerpts

> "Most current speech recognition systems use hidden Markov models (HMMs) to deal with the temporal variability of speech and Gaussian mixture models to determine how well each state of each HMM fits a frame or a short window of frames of coefficients that represents the acoustic input."
> ~ Abstract

> "Deep neural networks with many hidden layers, that are trained using new methods have been shown to outperform Gaussian mixture models on a variety of speech recognition benchmarks, sometimes by a large margin."
> ~ Abstract

> "This paper provides an overview of this progress and represents the shared views of four research groups who have had recent successes in using deep neural networks for acoustic modeling in speech recognition."
> ~ Abstract

## Reveals about tendency of thought

- Hinton treats cross-lab consensus as a way to validate a technique, rather than relying on a single group's results.
- The paper shows his consistent strategy of displacing a well-established statistical model, the Gaussian mixture model, with a learned neural alternative.
- It demonstrates his readiness to move deep learning results across domains, from vision into speech.

## Related

- [[10_Sources/Papers/geoffrey-hinton/imagenet-alexnet-2012|ImageNet Classification with Deep Convolutional Neural Networks]] - the parallel 2012 breakthrough in vision that established the same architectural shift.
- [[10_Sources/Papers/geoffrey-hinton/speech-recognition-deep-rnn-2013|Speech Recognition with Deep Recurrent Neural Networks]] - the follow-up recurrent architecture applied to the same task.
- [[20_People/geoffrey-hinton/profile|Geoffrey Hinton]]
