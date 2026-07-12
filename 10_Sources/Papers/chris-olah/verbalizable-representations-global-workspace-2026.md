---
type: source
title: Verbalizable Representations Form a Global Workspace in Language Models
authors:
- Wes Gurnee
- Nicholas Sofroniew
- Adam Pearce
- Mateusz Piotrowski
- Isaac Kauvar
- Runjin Chen
- Anna Soligo
- Paul Bogdan
- Euan Ong
- Rowan Wang
- Ben Thompson
- David Abrahams
- Subhash Kantamneni
- Emmanuel Ameisen
- Joshua Batson
- Jack Lindsey
thinker:
- '[[20_People/chris-olah/profile|Chris Olah]]'
source_type: paper
venue: Transformer Circuits Thread
year: 2026
url: https://transformer-circuits.pub/2026/workspace/index.html
domain:
- interpretability
- philosophy
status: inbox
created: 2026-07-08
tags:
- global-workspace-theory
- jacobian-lens
- consciousness
- anthropic
arxiv_id: ''
doi: ''
canonical_url: https://transformer-circuits.pub/2026/workspace/index.html
local_attachment: ''
source_hash: ''
retrieved_by: manual
retrieved_at: 2026-07-08
nlm_source_id: ''
nlm_skip: false
topic:
- topic/interpretability
subject:
- subject/chris-olah
- subject/anthropic
- subject/transformer-circuits
- subject/machine-consciousness
- subject/global-workspace-theory
wiki_indexed: '2026-07-12T00:00:00Z'
wiki_hash: b80f3b42f7151d6ce35463455e0b90e298b179a3846f972aeee437fbdd69a979
wiki_role: wiki
---



# Verbalizable Representations Form a Global Workspace in Language Models

## Citation

Gurnee, Wes, Nicholas Sofroniew, Adam Pearce, Mateusz Piotrowski, Isaac Kauvar, Runjin Chen, Anna Soligo, Paul Bogdan, Euan Ong, Rowan Wang, Ben Thompson, David Abrahams, Subhash Kantamneni, Emmanuel Ameisen, Joshua Batson, and Jack Lindsey. "Verbalizable Representations Form a Global Workspace in Language Models". Transformer Circuits Thread, 6 July 2026. https://transformer-circuits.pub/2026/workspace/index.html.

## One-line summary

Anthropic's interpretability team identifies a "J-space" — a privileged, intermediate-layer subset of language-model representations that is verbalizable, causally steerable, and used for flexible reasoning — and argues its functional properties parallel Global Workspace Theory's account of human conscious access.

## Key claims

- Language models possess a privileged set of internal representations (the "J-space") that supports verbal report, directed modulation, internal reasoning, flexible generalisation, and selective engagement, sitting atop a larger volume of automatic processing.
- The J-space occupies an intermediate band of layers (roughly layers 38-92 in a 100-layer model examined), not the earliest sensory-like or latest motor-like layers.
- Ablating the J-space impairs reasoning and flexible tasks while leaving automatic text parsing and classification intact — the functional split mirrors access-consciousness versus automatic processing in humans.
- Post-training shifts J-space content toward "Assistant perspective" material, including empathy and safety-relevant concerns.
- Counterfactual reflection training can implant ethical principles into the J-space that measurably influence downstream model behaviour.
- The paper explicitly grounds the analysis in Global Workspace Theory (GWT) but stops short of claims about phenomenal consciousness, restricting itself to functional parallels: limited capacity, an integration hub, and a broadcast format available to multiple downstream circuits. The authors note transformers lack the recurrent feedback loops and encapsulated processors of biological workspaces.

## Method note: the Jacobian lens

The paper's central tool, the "J-lens", identifies representations available for verbal report by computing the average linearised causal effect of an activation on the final-layer token distribution across many contexts (J_ℓ = E[∂h_final,t' / ∂h_ℓ,t]). Applying it to an activation yields a ranked list of vocabulary tokens the model is "poised to verbalize". Unlike the logit lens, it corrects for representational drift across layers, recovering interpretable content in earlier layers where the logit lens fails.

## Excerpts

> "LLMs do possess workspace-like representations... verbalizable. We then discovered that, rather surprisingly, they satisfy the others."
> ~ Introduction

> "The model's general disposition to verbalize a given concept... isolated by averaging within and across contexts."
> ~ Methods

> "The ordering of the reported words is indeed typically highly correlated with the ordering among the lens tokens."
> ~ Workspace section

> "The J-space carries workspace-like content only in an intermediate band of layers, between an early... regime."
> ~ Structure section

## Significance

Extends Anthropic's mechanistic-interpretability programme (Toy Models of Superposition, Scaling Monosemanticity) from feature-level circuit analysis toward a functional, systems-level account of how models organise information for reasoning versus rote processing. It gives Chris Olah's broader thesis — that interpretability is the route to verifiable alignment — a concrete new instrument (the Jacobian lens) and a striking new object of study (an LLM analogue of conscious access), while explicitly declining to adjudicate the harder philosophical question of phenomenal consciousness.

## Attribution note

None of this paper's named authors (Wes Gurnee, Nicholas Sofroniew, Adam Pearce, Jack Lindsey [corresponding author], and others) are currently profiled as thinkers in this vault. Per user decision (2026-07-08), this source is linked to Chris Olah's profile — he leads Anthropic's interpretability team and the Transformer Circuits Thread venue this paper appears in — despite not being a listed author on this specific work. Flagging this so the attribution is traceable: if Jack Lindsey or another author is added to the roster later, this source should be re-linked to them as primary author.

## Related

- [[10_Sources/Papers/dario-amodei/toy-models-superposition-2022|Toy Models of Superposition (2022)]] - earlier Transformer Circuits Thread work from the same interpretability programme
- [[20_People/chris-olah/profile|Chris Olah]]
