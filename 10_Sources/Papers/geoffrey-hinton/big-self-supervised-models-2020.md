---
type: source
title: Big Self-Supervised Models are Strong Semi-Supervised Learners
authors:
- Ting Chen
- Simon Kornblith
- Kevin Swersky
- Mohammad Norouzi
- Geoffrey Hinton
thinker:
- '[[20_People/geoffrey-hinton/profile|Geoffrey Hinton]]'
source_type: paper
venue: NeurIPS 2020
year: 2020
url: https://arxiv.org/abs/2006.10029
domain:
- capability
status: inbox
created: 2026-10-04
tags:
- self-supervised-learning
- semi-supervised-learning
- simclr
- distillation
arxiv_id: '2006.10029'
doi: ''
canonical_url: https://arxiv.org/abs/2006.10029
local_attachment: ''
source_hash: ''
retrieved_by: wiki-thinker-researcher
retrieved_at: 2026-10-04
nlm_source_id: ''
nlm_skip: false
topic:
- topic/knowledge-distillation
- topic/representation-learning
subject:
- subject/geoffrey-hinton
- subject/simclr
wiki_indexed: '2026-10-04T02:48:24Z'
wiki_hash: 3486d85d2b2e401d659664f631495830fb9ccba0ffe13de5baa3ab7d36736f50
wiki_role: wiki
---

# Big Self-Supervised Models are Strong Semi-Supervised Learners (2020)

## Citation

Chen, T., Kornblith, S., Swersky, K., Norouzi, M. and Hinton, G. "Big Self-Supervised Models are Strong Semi-Supervised Learners". NeurIPS 2020, 2020. https://arxiv.org/abs/2006.10029.

## One-line summary

The paper shows that a big self-supervised network, fine-tuned on few labels and then distilled using unlabelled data, gives large gains in label efficiency on ImageNet.

## Key claims

- Unsupervised pretraining followed by supervised fine-tuning is a standard way to learn from few labels.
- The fewer the labels, the more a bigger network helps.
- The method has three steps: SimCLRv2 pretraining, fine-tuning, and distillation with unlabelled examples.
- With 1% of labels, ResNet-50 reaches 73.9% top-1 accuracy on ImageNet.
- With 10% of labels, ResNet-50 reaches 77.5% and beats standard supervised training on all labels.

## Excerpts

> "One paradigm for learning from few labeled examples while making best use of a large amount of unlabeled data is unsupervised pretraining followed by supervised fine-tuning."
> ~ Abstract, arXiv 2006.10029

> "We find that, the fewer the labels, the more this approach (task-agnostic use of unlabeled data) benefits from a bigger network."
> ~ Abstract, arXiv 2006.10029

> "The proposed semi-supervised learning algorithm can be summarized in three steps: unsupervised pretraining of a big ResNet model using SimCLRv2, supervised fine-tuning on a few labeled examples, and distillation with unlabeled examples for refining and transferring the task-specific knowledge."
> ~ Abstract, arXiv 2006.10029

> "This procedure achieves 73.9% ImageNet top-1 accuracy with just 1% of the labels using ResNet-50, a 10× improvement in label efficiency over the previous state-of-the-art."
> ~ Abstract, arXiv 2006.10029

> "With 10% of labels, ResNet-50 trained with our method achieves 77.5% top-1 accuracy, outperforming standard supervised training with all of the labels."
> ~ Abstract, arXiv 2006.10029

## Reveals about tendency of thought

- Reads as a continuation of Hinton's long bet on unsupervised representation learning as the route to data-efficient intelligence.
- Suggests a preference for scaling model size as the lever, with distillation used to recover compact models afterwards.

## Related

- [[10_Sources/Papers/geoffrey-hinton/simclr-2020|A Simple Framework for Contrastive Learning of Visual Representations]] - the SimCLR method this work extends
- [[10_Sources/Papers/geoffrey-hinton/distilling-knowledge-2015|Distilling the Knowledge in a Neural Network]] - the distillation idea used in the third step
- [[20_People/geoffrey-hinton/profile|Geoffrey Hinton]]
