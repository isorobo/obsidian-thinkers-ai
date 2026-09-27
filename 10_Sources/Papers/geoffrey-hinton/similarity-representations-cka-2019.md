---
type: source
title: Similarity of Neural Network Representations Revisited
authors:
- Simon Kornblith
- Mohammad Norouzi
- Honglak Lee
- Geoffrey Hinton
thinker:
- '[[20_People/geoffrey-hinton/profile|Geoffrey Hinton]]'
source_type: paper
venue: Proceedings of the 36th International Conference on Machine Learning (ICML)
year: 2019
url: https://arxiv.org/abs/1905.00414
domain:
- interpretability
status: inbox
created: 2026-08-17
tags:
- representation-similarity
- interpretability
- cka
arxiv_id: '1905.00414'
doi: ''
canonical_url: https://arxiv.org/abs/1905.00414
local_attachment: ''
source_hash: ''
retrieved_by: wiki-thinker-researcher
retrieved_at: 2026-08-17
nlm_source_id: ''
nlm_skip: false
topic:
- topic/interpretability
- topic/representation-learning
subject:
- subject/geoffrey-hinton
- subject/simon-kornblith
- subject/centered-kernel-alignment
- subject/canonical-correlation-analysis
wiki_indexed: '2026-08-17T08:20:52Z'
wiki_hash: 17b34cdf2ec7bd733f527e389569dbae8ce41f6d840e3d67af8cd170b53da06d
wiki_role: wiki
---


# Similarity of Neural Network Representations Revisited

## Citation

Kornblith, S., Norouzi, M., Lee, H. and Hinton, G. "Similarity of Neural Network Representations Revisited". Proceedings of the 36th International Conference on Machine Learning, 2019, pp. 3519-3529. https://arxiv.org/abs/1905.00414.

## One-line summary

Kornblith, Norouzi, Lee, and Hinton introduce centered kernel alignment as a measure that reliably compares neural network representations across layers and models.

## Key claims

- Comparing representations between layers and between trained models helps explain neural network behaviour.
- Canonical correlation analysis, CCA, belongs to a broader family of statistics for measuring multivariate similarity.
- No statistic invariant to invertible linear transformation, including CCA, can meaningfully measure similarity between representations of higher dimension than the number of data points.
- The paper introduces a similarity index that measures the relationship between representational similarity matrices without this limitation.
- This index is equivalent to centered kernel alignment, CKA, and closely connected to CCA.
- Unlike CCA, CKA reliably identifies correspondences between representations in networks trained from different initialisations.

## Excerpts

> "Recent work has sought to understand the behavior of neural networks by comparing representations between layers and between different trained models."
> ~ Abstract

> "We show that CCA belongs to a family of statistics for measuring multivariate similarity, but that neither CCA nor any other statistic that is invariant to invertible linear transformation can measure meaningful similarities between representations of higher dimension than the number of data points."
> ~ Abstract

> "Unlike CCA, CKA can reliably identify correspondences between representations in networks trained from different initializations."
> ~ Abstract

## Reveals about tendency of thought

- Hinton treats interpretability of learned representations as a measurement problem requiring rigorous statistical justification.
- The paper shows willingness to overturn a widely used tool, CCA, once its mathematical limitations become clear.
- The focus on cross-initialisation comparison reflects his interest in what neural networks learn in common, not just what any single network learns.

## Related

- [[10_Sources/Papers/geoffrey-hinton/visualizing-tsne-2008|Visualizing Data using t-SNE]] - an earlier tool for inspecting learned representations.
- [[10_Sources/Papers/geoffrey-hinton/simclr-2020|A Simple Framework for Contrastive Learning of Visual Representations]] - a related paper with overlapping co-authors on representation quality.
- [[20_People/geoffrey-hinton/profile|Geoffrey Hinton]]
