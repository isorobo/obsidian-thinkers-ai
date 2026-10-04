---
type: source
title: Mechanistic anomaly detection and ELK
authors:
- Paul Christiano
- Mark Xu
thinker:
- '[[20_People/paul-christiano/profile|Paul Christiano]]'
source_type: essay
venue: ARC Blog (alignment.org)
year: 2022
url: https://www.alignment.org/blog/mechanistic-anomaly-detection-and-elk/
domain:
- alignment
- interpretability
status: inbox
created: 2026-10-04
tags:
- elk
- anomaly-detection
- mechanistic-explanations
- arc-theory
arxiv_id: ''
doi: ''
canonical_url: https://www.alignment.org/blog/mechanistic-anomaly-detection-and-elk/
local_attachment: ''
source_hash: ''
retrieved_by: wiki-thinker-researcher
retrieved_at: 2026-10-04
nlm_source_id: ''
nlm_skip: false
topic:
- topic/alignment
- topic/interpretability
wiki_indexed: '2026-10-04T03:18:02Z'
wiki_hash: 1e56445032800025d9db0d2815d6bfacf18b929a7cbb04d4fe5310502eff10f0
---

# Mechanistic anomaly detection and ELK (2022)

## Citation

Christiano, P. and Xu, M. "Mechanistic anomaly detection and ELK". ARC Blog, 25 November 2022. https://www.alignment.org/blog/mechanistic-anomaly-detection-and-elk/.

## One-line summary

The post proposes mechanistic anomaly detection, flagging outputs produced for unusual reasons, as a possible route to solving eliciting latent knowledge.

## Key claims

- Model behaviour should be explainable from the weights without reference to the training process.
- Variance on the training set is driven by variance in the model's underlying beliefs in the deceptive-alignment setting.
- A concrete test task is detecting inputs where the output is large because of a backdoor.
- Given explanations of key behaviours, the authors are tentatively optimistic about this route to ELK.

## Excerpts

> "The weights screen off the training process and so it should be possible to explain any given behavior of the model without reference to the training process."
> ~ ARC Blog, 25 November 2022, section on ELK and explanation

> "On the training set the variance is driven by variance in the model's underlying beliefs, holding fixed the decision to provide honest answers"
> ~ ARC Blog, 25 November 2022, section on deceptive alignment

> "The backdoor attack detection task is to detect inputs x* where f(x*) is large because of the backdoor"
> ~ ARC Blog, 25 November 2022, section on backdoor attack detection

> "If we are able to find explanations for the key model behaviors, we are tentatively optimistic about mechanistic anomaly detection as a way to solve ELK."
> ~ ARC Blog, 25 November 2022, conclusion

## Reveals about tendency of thought

- Reads as a habit of reducing a broad alignment problem to a precisely stated detection task with toy benchmarks.
- Suggests hedged optimism that depends on an unsolved prerequisite, finding explanations.

## Related

- [[20_People/paul-christiano/profile|Paul Christiano]]
