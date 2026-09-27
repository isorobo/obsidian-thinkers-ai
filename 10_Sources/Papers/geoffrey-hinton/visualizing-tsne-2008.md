---
type: source
title: Visualizing Data using t-SNE
authors:
- Laurens van der Maaten
- Geoffrey Hinton
thinker:
- '[[20_People/geoffrey-hinton/profile|Geoffrey Hinton]]'
source_type: paper
venue: Journal of Machine Learning Research
year: 2008
url: https://jmlr.org/papers/v9/vandermaaten08a.html
domain:
- interpretability
status: inbox
created: 2026-08-17
tags:
- t-sne
- visualization
- dimensionality-reduction
arxiv_id: ''
doi: ''
canonical_url: https://jmlr.org/papers/v9/vandermaaten08a.html
local_attachment: ''
source_hash: ''
retrieved_by: wiki-thinker-researcher
retrieved_at: 2026-08-17
nlm_source_id: ''
nlm_skip: false
topic:
- topic/representation-learning
subject:
- subject/geoffrey-hinton
- subject/laurens-van-der-maaten
- subject/t-sne
wiki_indexed: '2026-08-17T08:20:52Z'
wiki_hash: 3599b1a68795b5d96d43df4912bf8702163aec06b435db36d4ce68d0ab429b21
wiki_role: wiki
---


# Visualizing Data using t-SNE

## Citation

van der Maaten, L. and Hinton, G. "Visualizing Data using t-SNE". Journal of Machine Learning Research, 9, 2008, pp. 2579-2605. https://jmlr.org/papers/v9/vandermaaten08a.html.

## One-line summary

Van der Maaten and Hinton introduce t-SNE, a technique that maps high-dimensional data onto two or three dimensions while preserving local structure.

## Key claims

- t-SNE gives each datapoint a location in a two or three-dimensional map derived from high-dimensional data.
- The technique is a variant of Stochastic Neighbor Embedding, easier to optimise and less prone to crowding points at the map centre.
- t-SNE reveals structure at many different scales within a single map, unlike prior linear methods.
- The paper extends t-SNE to large datasets using random-walk-based approximations.
- Comparisons show t-SNE outperforms Sammon mapping, Isomap, and Locally Linear Embedding on standard benchmarks.

## Excerpts

> "We present a new technique called 't-SNE' that visualizes high-dimensional data by giving each datapoint a location in a two or three-dimensional map."
> ~ Abstract

> "This is a variation of Stochastic Neighbor Embedding (Hinton and Roweis, 2002) that is much easier to optimize and produces significantly better visualizations by reducing the tendency to crowd points together in the center of the map."
> ~ Abstract

> "t-SNE is better than existing techniques at creating a single map that reveals structure at many different scales."
> ~ Abstract

## Reveals about tendency of thought

- Hinton treats visualisation of learned representations as a research problem in its own right, not an afterthought.
- The work continues his 2002 Stochastic Neighbor Embedding line, showing sustained iteration on a single idea over years.
- The emphasis on multi-scale structure reflects his broader interest in hierarchical representation.

## Related

- [[10_Sources/Papers/geoffrey-hinton/reducing-dimensionality-2006|Reducing the Dimensionality of Data with Neural Networks]] - the companion dimensionality-reduction result from the same period.
- [[10_Sources/Papers/geoffrey-hinton/similarity-representations-cka-2019|Similarity of Neural Network Representations Revisited]] - later work on comparing learned representations.
- [[20_People/geoffrey-hinton/profile|Geoffrey Hinton]]
