---
type: source
title: Rectified Linear Units Improve Restricted Boltzmann Machines
authors:
- Vinod Nair
- Geoffrey E. Hinton
thinker:
- '[[20_People/geoffrey-hinton/profile|Geoffrey Hinton]]'
source_type: paper
venue: Proceedings of the 27th International Conference on Machine Learning (ICML)
year: 2010
url: https://dl.acm.org/doi/10.5555/3104322.3104425
domain:
- capability
status: inbox
created: 2026-08-17
tags:
- relu
- restricted-boltzmann-machines
- activation-functions
arxiv_id: ''
doi: ''
canonical_url: https://www.cs.toronto.edu/~hinton/absps/reluICML.pdf
local_attachment: ''
source_hash: ''
retrieved_by: wiki-thinker-researcher
retrieved_at: 2026-08-17
nlm_source_id: ''
nlm_skip: false
topic:
- topic/training-dynamics
subject:
- subject/geoffrey-hinton
- subject/vinod-nair
- subject/rectified-linear-units
- subject/restricted-boltzmann-machines
- subject/norb
- subject/labeled-faces-in-the-wild
wiki_indexed: '2026-08-17T08:20:52Z'
wiki_hash: 786b1c74267e3f61f0e7f15c16a15dd754d7a301989cc03d9a9751c50ca5802f
wiki_role: wiki
---


# Rectified Linear Units Improve Restricted Boltzmann Machines

## Citation

Nair, V. and Hinton, G. E. "Rectified Linear Units Improve Restricted Boltzmann Machines". Proceedings of the 27th International Conference on Machine Learning, 2010, pp. 807-814. https://dl.acm.org/doi/10.5555/3104322.3104425.

## One-line summary

Nair and Hinton replace binary stochastic hidden units in restricted Boltzmann machines with rectified linear units, improving object and face recognition.

## Key claims

- Restricted Boltzmann machines traditionally use binary stochastic hidden units.
- Binary units generalise to an infinite set of copies at progressively more negative biases, termed Stepped Sigmoid Units.
- Stepped Sigmoid Units are efficiently approximated by noisy, rectified linear units.
- Rectified linear units learn features that improve object recognition on the NORB dataset relative to binary units.
- The same units improve face verification accuracy on the Labeled Faces in the Wild benchmark.

## Excerpts

> "Restricted Boltzmann machines were developed using binary stochastic hidden units."
> ~ Abstract

> "These can be generalized by replacing each binary unit by an infinite number of copies that all have the same weights but with progressively more negative biases."
> ~ Abstract

> "Compared with binary units, these units learn features that are better for object recognition on the NORB dataset and face verification on the Labeled Faces in the Wild dataset."
> ~ Abstract

## Reveals about tendency of thought

- Hinton pursues small architectural substitutions with outsized downstream effects, a pattern that recurs across his career.
- The paper reflects his willingness to popularise components later found essential elsewhere in deep learning, well before their broader adoption.
- The choice of two disparate benchmarks, objects and faces, shows a preference for testing generality rather than a single task.

## Related

- [[10_Sources/Papers/geoffrey-hinton/deep-boltzmann-machines-2009|Deep Boltzmann Machines]] - the multi-layer Boltzmann machine framework this paper's units improve.
- [[10_Sources/Papers/geoffrey-hinton/dropout-2014|Improving neural networks by preventing co-adaptation of feature detectors]] - a related regularisation innovation from the same research programme.
- [[20_People/geoffrey-hinton/profile|Geoffrey Hinton]]
