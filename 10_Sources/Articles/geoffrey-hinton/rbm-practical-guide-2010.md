---
type: source
title: A Practical Guide to Training Restricted Boltzmann Machines
authors:
- Geoffrey Hinton
thinker:
- '[[20_People/geoffrey-hinton/profile|Geoffrey Hinton]]'
source_type: essay
venue: University of Toronto (UTML TR 2010-003)
year: 2010
url: https://www.cs.toronto.edu/~hinton/absps/guideTR.pdf
domain:
- capability
status: verified
created: 2026-06-07
tags:
- restricted-boltzmann-machines
- contrastive-divergence
- training-heuristics
- technical-report
arxiv_id: ''
doi: ''
canonical_url: https://www.cs.toronto.edu/~hinton/absps/guideTR.pdf
local_attachment: ''
source_hash: ''
retrieved_by: wiki-thinker-researcher
retrieved_at: 2026-06-07
nlm_source_id: ''
topic:
- topic/training-dynamics
subject:
- subject/geoffrey-hinton
- subject/restricted-boltzmann-machines
- subject/contrastive-divergence
wiki_indexed: '2026-06-14T12:00:00Z'
wiki_hash: ef2254c92105fce2f1e360635351334a2faa08256b8bd6e41b71ef96b894255d
wiki_role: raw
---



# A Practical Guide to Training Restricted Boltzmann Machines (2010)

## Citation

Hinton, Geoffrey. "A Practical Guide to Training Restricted Boltzmann Machines, Version 1". UTML TR 2010-003, Department of Computer Science, University of Toronto, 2 August 2010. https://www.cs.toronto.edu/~hinton/absps/guideTR.pdf.

## One-line summary

Hinton sets out the practical heuristics his Toronto group developed for training restricted Boltzmann machines with contrastive divergence, framing the document as a living guide for novice users.

## Key claims

- The most important use of RBMs is as learning modules composed to form deep belief nets.
- RBMs are usually trained with the contrastive divergence learning procedure.
- Training requires practical experience to set meta-parameters such as learning rate, momentum, weight-cost, sparsity target, and mini-batch size.
- Published code specifies the decisions but does not explain why they were made or how changes affect performance.
- The guide shares the Toronto group's accumulated expertise with other researchers.
- The document is a living one that will be updated, so its version number should always be cited.

## Excerpts

> "Their most important use is as learning modules that are composed to form deep belief nets."
~ "1 Introduction", UTML TR 2010-003

> "RBMs are usually trained using the contrastive divergence learning procedure."
~ "1 Introduction", UTML TR 2010-003

> "For any particular application, the code that was used gives a complete specification of all of these decisions, but it does not explain why the decisions were made or how minor changes will affect performance."
~ "1 Introduction", UTML TR 2010-003

> "Over the last few years, the machine learning group at the University of Toronto has acquired considerable expertise at training RBMs and this guide is an attempt to share this expertise with other machine learning researchers."
~ "1 Introduction", UTML TR 2010-003

> "We are still on a fairly steep part of the learning curve, so the guide is a living document that will be updated from time to time and the version number should always be used when referring to it."
~ "1 Introduction", UTML TR 2010-003

## Reveals about tendency of thought

- Craft over formalism: Hinton writes a guide of heuristics and recipes, treating training as a practical skill rather than a closed theory.
- Teaching reflex: the document exists to transfer tacit lab knowledge to newcomers, a recurring strand in his career.
- Honest uncertainty: he calls the field a steep learning curve and the text a living document, declining false finality.
- Reproducibility concern: he notes that code alone hides the reasoning behind design choices, so he supplies the reasoning.

## Related

- [[20_People/geoffrey-hinton/profile|Geoffrey Hinton]]
- [[10_Sources/Papers/geoffrey-hinton/deep-belief-nets-2006|A fast learning algorithm for deep belief nets]]
- [[10_Sources/Papers/geoffrey-hinton/dropout-2014|Improving neural networks by preventing co-adaptation of feature detectors]]
- [[20_People/yoshua-bengio/profile|Yoshua Bengio]]
