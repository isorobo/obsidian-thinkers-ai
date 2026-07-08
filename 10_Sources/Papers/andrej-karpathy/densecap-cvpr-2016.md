---
type: source
title: 'DenseCap: Fully Convolutional Localization Networks for Dense Captioning'
authors:
- Justin Johnson
- Andrej Karpathy
- Fei-Fei Li
thinker:
- '[[20_People/andrej-karpathy/profile|Andrej Karpathy]]'
source_type: paper
venue: CVPR 2016
year: 2016
url: https://arxiv.org/abs/1511.07571
domain:
- capability
- vision-language
status: inbox
created: 2026-06-21
tags:
- dense-captioning
- computer-vision
- image-captioning
- localization
arxiv_id: '1511.07571'
doi: ''
canonical_url: https://arxiv.org/abs/1511.07571
local_attachment: ''
source_hash: ''
retrieved_by: wiki-thinker-researcher
retrieved_at: 2026-06-21
nlm_source_id: ''
nlm_skip: false
topic:
- topic/convnets
- topic/representation-learning
- topic/vision-language
subject:
- subject/andrej-karpathy
- subject/fei-fei-li
- subject/dense-captioning
- subject/visual-genome
- subject/object-detection
wiki_indexed: '2026-06-21T18:30:00Z'
wiki_hash: b40df1bcb1165697aa9347e15b3061a625284f2e82900bec64442d206432424f
wiki_role: wiki
---


# DenseCap: Fully Convolutional Localization Networks for Dense Captioning

## Citation

Justin Johnson, Andrej Karpathy, Fei-Fei Li. "DenseCap: Fully Convolutional Localization Networks for Dense Captioning". CVPR 2016 (Oral). https://arxiv.org/abs/1511.07571.

## One-line summary

Johnson, Karpathy, and Li introduce dense captioning - the task of simultaneously localising and describing multiple image regions in natural language - using a single end-to-end network.

## Key claims

- Dense captioning unifies object detection and image captioning as special cases of a single task.
- The Fully Convolutional Localization Network processes an image in one forward pass without external region proposals.
- The architecture combines a convolutional network, a novel localization layer, and an RNN language model trained jointly end-to-end.
- The Visual Genome dataset (94,000 images, 4.1 million region-grounded captions) supports training and evaluation.
- The approach outperforms pipeline-based comparable methods in both generation and retrieval metrics.

## Excerpts

> "We present the dense captioning task, which requires a computer vision system to both localize and describe salient regions in images in natural language."
> ~ Abstract

> "Our architecture processes an image with a single, efficient forward pass, and the entire system is trained end-to-end."
> ~ Abstract

> "Dense captioning subsumes object detection as a special case (use single-word descriptions) and image captioning as a special case (use a single region that covers the full image)."
> ~ Introduction

## Reveals about tendency of thought

- Karpathy pursues architectural unification: collapsing distinct tasks (detection, captioning) into one model reflects his preference for elegant single-system solutions over pipelines.
- End-to-end training is a recurring design principle. The paper eliminates hand-engineered region proposals in favour of joint optimisation, consistent with his Software 2.0 thesis that neural networks should absorb entire engineering stacks.
- Joint work with Fei-Fei Li during his Stanford PhD years shows the vision-language alignment focus that defined his early research programme.

## Related

- [[10_Sources/Papers/andrej-karpathy/deep-visual-semantic-alignments-2015|Deep Visual-Semantic Alignments (2015)]] - earlier work on image-sentence alignment
- [[10_Sources/Papers/andrej-karpathy/deep-fragment-embeddings-2014|Deep Fragment Embeddings (2014)]] - bidirectional image-sentence mapping
- [[10_Sources/Articles/andrej-karpathy/software-2-0|Software 2.0 (2017)]] - essays that generalise this architectural philosophy
