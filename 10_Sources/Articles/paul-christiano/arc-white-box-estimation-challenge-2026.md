---
type: source
title: Announcing the ARC White-Box Estimation Challenge
authors:
- Jacob Hilton
- Paul Christiano
- Wilson Wu
thinker:
- '[[20_People/paul-christiano/profile|Paul Christiano]]'
source_type: essay
venue: ARC Blog (alignment.org)
year: 2026
url: https://www.alignment.org/blog/announcing-the-arc-white-box-estimation-challenge/
domain:
- interpretability
- alignment
status: inbox
created: 2026-10-04
tags:
- arc-theory
- mechanistic-estimation
- contest
- random-mlps
arxiv_id: ''
doi: ''
canonical_url: https://www.alignment.org/blog/announcing-the-arc-white-box-estimation-challenge/
local_attachment: ''
source_hash: ''
retrieved_by: wiki-thinker-researcher
retrieved_at: 2026-10-04
nlm_source_id: ''
nlm_skip: false
topic:
- topic/interpretability
wiki_indexed: '2026-10-04T03:18:02Z'
wiki_hash: 147025d1a53651c48266b059e1cb1ba29a8a3dba74a219456b72ec9004df91fd
---

# Announcing the ARC White-Box Estimation Challenge (2026)

## Citation

Hilton, J., Christiano, P. and Wu, W. "Announcing the ARC White-Box Estimation Challenge". ARC Blog, 2 June 2026. https://www.alignment.org/blog/announcing-the-arc-white-box-estimation-challenge/.

## One-line summary

ARC announces a contest in which entrants design algorithms that estimate the expected output of random MLPs from the weights alone, as a testbed for white-box reasoning about AI systems.

## Key claims

- Contestants must design an algorithm that takes a set of weights and estimates the expected output.
- Algorithms are scored on MLPs with randomly sampled Gaussian weights by mean squared error.
- The long-run motivation is answering questions about highly intelligent AI systems.
- Contestants are encouraged to use LLMs.

## Excerpts

> "Contestants must design an algorithm that takes in a set of weights θ and produces an estimate for the expected output"
> ~ ARC Blog, 2 June 2026, challenge scope

> "Algorithms will be evaluated on MLPs with randomly-sampled Gaussian weights. The goal is to achieve as low mean squared error as possible"
> ~ ARC Blog, 2 June 2026, evaluation criteria

> "In the long run, we would like to answer questions about highly intelligent AI systems such as, 'Are there unusual situations in which the system would undermine human control?'"
> ~ ARC Blog, 2 June 2026, motivation

> "We encourage contestants to use LLMs to whatever extent helps them improve their submissions the most. In later rounds, there will be two kinds of prize"
> ~ ARC Blog, 2 June 2026, LLM usage policy

## Reveals about tendency of thought

- Suggests ARC treats a clean toy estimation problem as the route to the practical goal of detecting loss of human control.
- Reads as a willingness to open theory problems to outside contestants.

## Related

- [[20_People/paul-christiano/profile|Paul Christiano]]
