---
type: source
title: Supervising strong learners by amplifying weak experts
authors:
- Paul Christiano
- Buck Shlegeris
- Dario Amodei
thinker:
- '[[20_People/paul-christiano/profile|Paul Christiano]]'
source_type: paper
venue: arXiv preprint
year: 2018
url: https://arxiv.org/abs/1810.08575
domain:
- alignment
- scalable-oversight
- safety
status: inbox
created: 2026-06-07
tags:
- iterated-amplification
- scalable-oversight
- expert-iteration
- openai
arxiv_id: '1810.08575'
doi: ''
canonical_url: https://arxiv.org/abs/1810.08575
local_attachment: ''
source_hash: ''
retrieved_by: wiki-thinker-researcher
retrieved_at: 2026-06-07
nlm_source_id: ''
nlm_skip: false
topic:
- topic/iterated-amplification
- topic/scalable-oversight
- topic/alignment
subject:
- subject/paul-christiano
- subject/iterated-amplification
wiki_indexed: '2026-06-07T10:00:00Z'
wiki_hash: 54bd14d9de1dc632de69bcb1c520aeb28480683be3b6c7d49a71f3c54fbf9ce5
wiki_role: wiki
---


# Supervising strong learners by amplifying weak experts

## Citation

Christiano, Paul, Buck Shlegeris, and Dario Amodei. "Supervising strong learners by amplifying weak experts". arXiv preprint, 2018. https://arxiv.org/abs/1810.08575.

## One-line summary

The paper introduces Iterated Amplification, which builds a training signal for hard problems by composing solutions to easier subproblems, without any external reward function.

## Key claims

- Hard-to-specify objectives produce poor performance or misaligned behaviour when replaced by easier proxies.
- Human demonstration or judgement fails once a task grows too complex for direct human evaluation.
- Iterated Amplification progressively assembles a training signal by combining solutions to easier subproblems.
- The method resembles Expert Iteration but uses no external reward function.
- Experiments in algorithmic environments show the method learning complex behaviours efficiently.

## Excerpts

> "We propose Iterated Amplification, an alternative training strategy which progressively builds up a training signal for difficult problems by combining solutions to easier subproblems."
> ~ Abstract

> "Iterated Amplification is closely related to Expert Iteration (Anthony et al., 2017; Silver et al., 2017), except that it uses no external reward function."
> ~ Abstract

> "We present results in algorithmic environments, showing that Iterated Amplification can efficiently learn complex behaviors."
> ~ Abstract

## Reveals about tendency of thought

- Amplification expresses Christiano's central bet: align a weak supervisor first, then bootstrap to stronger systems without ever needing a reward the human cannot evaluate.
- The decomposition strategy mirrors how he reasons in essays, breaking a hard alignment question into checkable parts.
- Removing the external reward function shows his worry that misspecified rewards drive misaligned behaviour.

## Related

- [[10_Sources/Papers/paul-christiano/ai-safety-via-debate-2018|AI safety via debate (2018)]] - sibling scalable-oversight mechanism
- [[10_Sources/Media/paul-christiano/ea-global-current-work-2019|Current work in AI alignment (EA Global 2019)]] - talk situating amplification in his agenda
- [[20_People/paul-christiano/profile|Paul Christiano]]
