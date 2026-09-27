---
type: source
title: A Simple Framework for Contrastive Learning of Visual Representations
authors:
- Ting Chen
- Simon Kornblith
- Mohammad Norouzi
- Geoffrey Hinton
thinker:
- '[[20_People/geoffrey-hinton/profile|Geoffrey Hinton]]'
source_type: paper
venue: Proceedings of the 37th International Conference on Machine Learning (ICML)
year: 2020
url: https://arxiv.org/abs/2002.05709
domain:
- capability
status: inbox
created: 2026-08-17
tags:
- contrastive-learning
- self-supervised-learning
- simclr
arxiv_id: '2002.05709'
doi: ''
canonical_url: https://arxiv.org/abs/2002.05709
local_attachment: ''
source_hash: ''
retrieved_by: wiki-thinker-researcher
retrieved_at: 2026-08-17
nlm_source_id: ''
nlm_skip: false
topic:
- topic/representation-learning
- topic/computer-vision
subject:
- subject/geoffrey-hinton
- subject/ting-chen
- subject/simon-kornblith
- subject/simclr
- subject/contrastive-learning
- subject/imagenet
- subject/google-brain
wiki_indexed: '2026-08-17T08:20:52Z'
wiki_hash: fe1c91701e315d678d89d30ec97c9a13adcab618fc7b6ae751a950d0a6cf7cf1
wiki_role: wiki
---


# A Simple Framework for Contrastive Learning of Visual Representations

## Citation

Chen, T., Kornblith, S., Norouzi, M. and Hinton, G. "A Simple Framework for Contrastive Learning of Visual Representations". Proceedings of the 37th International Conference on Machine Learning, 2020. https://arxiv.org/abs/2002.05709.

## One-line summary

Chen, Kornblith, Norouzi, and Hinton present SimCLR, a contrastive self-supervised framework that matches supervised ResNet-50 performance without labels.

## Key claims

- SimCLR simplifies contrastive self-supervised learning without specialised architectures or a memory bank.
- Composition of data augmentations plays a critical role in defining effective predictive tasks.
- A learnable nonlinear transformation between representation and contrastive loss substantially improves representation quality.
- Contrastive learning benefits more from larger batch sizes and longer training than supervised learning does.
- A linear classifier trained on SimCLR representations reaches 76.5% top-1 accuracy on ImageNet, matching supervised ResNet-50.
- Fine-tuned on 1% of labels, the model reaches 85.8% top-5 accuracy, beating AlexNet trained with 100 times more labels.

## Excerpts

> "We simplify recently proposed contrastive self-supervised learning algorithms without requiring specialized architectures or a memory bank."
> ~ Abstract

> "Introducing a learnable nonlinear transformation between the representation and the contrastive loss substantially improves the quality of the learned representations."
> ~ Abstract

> "A linear classifier trained on self-supervised representations learned by SimCLR achieves 76.5% top-1 accuracy, which is a 7% relative improvement over previous state-of-the-art, matching the performance of a supervised ResNet-50."
> ~ Abstract

## Reveals about tendency of thought

- Hinton continues to push self-supervised learning as a route to reducing dependence on labelled data.
- The paper shows a systematic, ablation-driven method: isolate each component's contribution before claiming an overall result.
- The comparison against a fully supervised baseline reflects his consistent habit of benchmarking new methods against the strongest existing alternative.

## Related

- [[10_Sources/Papers/geoffrey-hinton/distilling-knowledge-2015|Distilling the Knowledge in a Neural Network]] - an earlier representation-transfer technique from the same research lineage.
- [[10_Sources/Papers/geoffrey-hinton/similarity-representations-cka-2019|Similarity of Neural Network Representations Revisited]] - a companion tool for analysing learned representations with the same co-authors.
- [[20_People/geoffrey-hinton/profile|Geoffrey Hinton]]
