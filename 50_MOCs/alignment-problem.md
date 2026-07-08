---
type: moc
title: The Alignment Problem - Views from AI Researchers
domain:
  - alignment
  - safety
status: permanent
created: 2026-06-30
updated: 2026-07-08
---

# The Alignment Problem: Views from AI Researchers

A synthesis of thinker positions on whether AI alignment is a solvable engineering problem, a deep philosophical challenge, or an open empirical question. Covers both difficulty and proposed solution paths.

## 1. Alignment as Engineering Problem (Tractable with Effort)

This camp views alignment as a solvable technical problem. Difficulty is real but not fundamental.

**Dario Amodei** [[20_People/dario-amodei/profile|dario-amodei]]: Alignment is tractable with effort. Invested heavily in mechanistic interpretability under Chris Olah. Authored the Responsible Scaling Policy framework as a voluntary commitment mechanism. Framing: continuous capability scaling + careful safety research = controllable systems. Key papers: [[10_Sources/Papers/dario-amodei/constitutional-ai-harmlessness-from-ai-feedback-2022|Constitutional AI: Harmlessness from AI Feedback (2022)]], [[10_Sources/Papers/dario-amodei/learning-to-summarize-from-human-feedback-2020|Learning to Summarize from Human Feedback (2020)]].

**Paul Christiano** [[20_People/paul-christiano/profile|paul-christiano]]: Alignment tractable through preference-learning and latent-knowledge elicitation. Default trajectory without serious effort is bad; but evaluations and compute governance buy time. Eliciting Latent Knowledge (ELK) is the central unsolved problem, not an intractable one. Key paper: [[10_Sources/Papers/paul-christiano/elk-2021|Eliciting Latent Knowledge (2021)]]. Related: [[10_Sources/Papers/paul-christiano/rlhf-2017|Deep Reinforcement Learning from Human Preferences (2017)]].

**Chris Olah** [[20_People/chris-olah/profile|chris-olah]]: Mechanistic interpretability offers a path to verifiable safety. Interpretability is not decorative; it is the only route to verifiable alignment. Progression from toy features to real circuits to scalable automation. Each stage delivers measurable outcomes. Key papers: [[10_Sources/Papers/chris-olah/scaling-laws-interpretability-repeated-data-2022|Scaling Laws for Interpretability on Repeatedly Trained Data (2022)]].

### Consensus within this camp

- Alignment requires intentional research effort, not hope.
- Interpretability, RLHF, and evaluations are complementary tools.
- Scaling policy commitments (RSPs, evaluations, red-teaming) can reduce risk whilst research progresses.
- The problem is hard but not intractable.

---

## 2. Alignment as Philosophical / Conceptual Problem (Hard, Possibly Fundamental)

This camp sees alignment as touching deep questions about value, agency, and control that resist engineering fixes alone.

**Geoffrey Hinton** [[20_People/geoffrey-hinton/profile|geoffrey-hinton]]: Existential risk plausible; default outcome uncertain. Assigns non-trivial probability to extinction-scale outcomes. Framing: once models become agentic and develop sub-goal reasoning, alignment becomes a control problem, not a training problem. Key talks: [[10_Sources/Media/geoffrey-hinton/60-minutes-2023|60 Minutes Interview (2023)]], [[10_Sources/Media/geoffrey-hinton/mit-tech-review-2023|MIT Technology Review (2023)]].

**Yoshua Bengio** [[20_People/yoshua-bengio/profile|yoshua-bengio]]: Alignment hard under agentic paradigms. Advocates scientist AI over agentic AI precisely because the latter carries irreducible loss-of-control risk. Framing: if we insist on autonomous agentic systems, alignment becomes harder than engineering. But non-agentic AI (scientist AI, tool AI) is tractable. International AI Safety Report (2025) reflects this position.

**Gary Marcus** [[20_People/gary-marcus/profile|gary-marcus]]: Misaligned to wrong problem; reliability before alignment. LLMs are unreliable and hallucinate; scaling does not fix this. Focus on reliability and robustness first. Alignment literature assumes models will be competent; that assumption is premature. Key paper: [[10_Sources/Papers/gary-marcus/gpt-3-commonsense-reasoning-tests-2020|GPT-3: Commonsense Reasoning Tests (2020)]].

### Consensus within this camp

- Alignment is not purely an engineering problem.
- Agentic systems carry irreducible loss-of-control risks.
- Precaution (non-agentic architectures, governance, pausing) may be necessary.
- The problem touches philosophy (what is value?), control theory (can we verify non-deception?), and institutional design (can labs self-regulate?).

---

## 3. Alignment as Open Question (Unknown or Deferred)

This camp treats alignment difficulty as empirically uncertain or explicitly defers to other thinkers.

**Andrej Karpathy** [[20_People/andrej-karpathy/profile|andrej-karpathy]]: Engineering problem; emergent behaviours observable with care. Framing: alignment is a design and testing problem, like autopilot. Observability and evals scale with capability. Does not focus on existential alignment risk; treats it as downstream of capability understanding. Key talks: [[10_Sources/Media/andrej-karpathy/state-of-gpt-2023|State of GPT (2023)]], [[10_Sources/Media/andrej-karpathy/intro-to-large-language-models-2023|Intro to Large Language Models (2023)]].

**Chris Olah** [[20_People/chris-olah/profile|chris-olah]]: Focuses on interpretability readiness rather than debating takeoff or alignment difficulty. Treats dynamics as secondary to transparency tooling. Implicitly: if we can inspect models, alignment is tractable.

**Erik Brynjolfsson** [[20_People/erik-brynjolfsson/profile|erik-brynjolfsson]]: Not primary focus; favours complementarity framing. Treats alignment as less central than distributional impacts of automation. Policy focus is on human-complementary AI design, not alignment per se.

**Yann LeCun** [[20_People/yann-lecun/profile|yann-lecun]]: Not existential; objective-driven architectures solve it by design. Framing: the problem is a systems-design question, not a safety research question. Build agents with well-defined objectives; bad alignment is a failure to specify objectives, not a control problem.

**Daron Acemoglu** [[20_People/daron-acemoglu/profile|daron-acemoglu]]: Not his focus; emphasises governance and distribution. Economic institutions and labour policy matter more than alignment research. Implicit position: alignment is a governance problem, not a research problem.

### Consensus within this camp

- Either alignment is not the central risk, or it is orthogonal to their primary focus.
- Design matters (Karpathy, LeCun: build the right architecture).
- Governance and distribution matter as much as technical alignment (Acemoglu).
- The problem may be overstated by x-risk researchers; we don't know yet.

---

## 4. Key Disagreements

### On agentic AI

**Hinton and Bengio vs. LeCun and Karpathy**: Hinton and Bengio worry that agentic AI *is* the trajectory and control is fragile. LeCun argues the trajectory is non-agentic (world models + objective-driven agents, not autonomous reasoning). Karpathy stays agnostic; agents arise from scale.

**Bengio's "scientist AI" thesis**: Argues we can constrain AI to non-agentic scientist roles (hypothesis generation, experiment design, analysis). Hinton agrees this is safer; Geoffrey-leans toward "we probably cannot build non-agentic advanced AI." Yann asserts we should and must.

### On interpretability as sufficient

**Olah and Amodei vs. others**: Olah and Amodei bet on mechanistic interpretability scaling to powerful models. Christiano is more uncertain (ELK is open). Hinton and Bengio are sceptical that interpretability prevents deception by an advanced agent. Gary Marcus argues interpretability without reliability is decorative.

### On the problem's frame

**Marcus's outlier position**: "Reliability before alignment." Current LLMs are not reliable; alignment is premature. Others treat reliability as a precondition *and* a component of alignment.

**Acemoglu's reframe**: Alignment is institutional (labour markets, capital distribution) not technical. Governance and economic incentives shape AI outcomes more than safety research.

---

## 5. Representative Sources

### Pro-alignment tractability

**Dario Amodei**:
- [[10_Sources/Papers/dario-amodei/concrete-problems-in-ai-safety|Concrete Problems in AI Safety (2016)]] — framing agenda
- [[10_Sources/Articles/dario-amodei/machines-of-loving-grace|Machines of Loving Grace (2024)]] — positive-case manifesto
- [[10_Sources/Media/dario-amodei/senate-testimony-2023|US Senate Testimony (2023)]] — policy + safety integration

**Paul Christiano**:
- [[10_Sources/Papers/paul-christiano/elk-2021|Eliciting Latent Knowledge (2021)]]
- [[10_Sources/Articles/paul-christiano/what-failure-looks-like|What failure looks like]] — concrete failure scenarios
- [[10_Sources/Media/paul-christiano/dwarkesh-preventing-ai-takeover-2023|Dwarkesh Podcast (2023)]]

**Chris Olah**:
- [[10_Sources/Papers/chris-olah/general-language-assistant-laboratory-alignment-2021|A General Language Assistant as a Laboratory for Alignment (2021)]]
- [[10_Sources/Articles/chris-olah/neural-networks-open-inspection|Neural Networks Can Be Open to Inspection]]

### Existential risk / control-problem framing

**Geoffrey Hinton**:
- [[10_Sources/Media/geoffrey-hinton/mit-tech-review-2023|MIT Technology Review Interview (2023)]]
- [[10_Sources/Media/geoffrey-hinton/nobel-interview-2024|Nobel Prize Interview (2024)]]
- [[10_Sources/Media/geoffrey-hinton/60-minutes-2023|60 Minutes (2023)]]

**Yoshua Bengio**:
- [[10_Sources/Papers/yoshua-bengio/international-ai-safety-report-2025|International AI Safety Report (2025)]] — scientist-AI case for non-agentic path
- [[20_People/yoshua-bengio/profile|Yoshua Bengio profile]] — Mila public advocacy

### Architecture-dependent optimism

**Yann LeCun**:
- [[10_Sources/Papers/yann-lecun/path-towards-autonomous-machine-intelligence-2022|Path Towards Autonomous Machine Intelligence (2022)]] — JEPA vision
- [[20_People/yann-lecun/profile|Yann LeCun profile]] — on objective-driven architectures

**Gary Marcus**:
- [[10_Sources/Books/gary-marcus/rebooting-ai-2019|Rebooting AI (2019)]] — neurosymbolic case
- [[10_Sources/Papers/gary-marcus/deep-learning-a-critical-appraisal-2018|Deep Learning: A Critical Appraisal (2018)]]

---

## 6. Unresolved Tensions

### Can we verify non-deception?

Christiano's ELK and Olah's interpretability assume that we can inspect models and confirm they are not deceiving us. Hinton is sceptical: sufficiently advanced systems may hide their goals. This is a *verification* problem, not a safety-research problem.

### Is agentic AI inevitable?

Bengio argues we should constrain ourselves to non-agentic AI. LeCun agrees this is possible and desirable. Hinton is pessimistic: autonomous agency emerges from scale. Karpathy is uncertain.

### Does interpretability scale?

Olah's research scales interpretability from toy models to real circuits. Open question: does it scale to frontier models with trillions of parameters? Affirmative assumption is not yet empirically confirmed.

### Is alignment the central safety problem?

Marcus argues reliability, robustness, and failure modes come first. Acemoglu argues distribution and governance are primary. Hinton argues loss of control. They are not contradictory, but they imply different research priorities.

---

## 7. The Alignment Spectrum (Mapped)

| **Thinker** | **Problem framing** | **Tractability** | **Policy implication** |
|---|---|---|---|
| Olah | Engineering (interpretability) | Tractable | Transparency standards |
| Amodei | Engineering + policy (RSPs) | Tractable | Compute + regulatory floor |
| Christiano | Engineering (preference learning) | Tractable with governance | Evaluations + compute-thresholds |
| Karpathy | Engineering (observability) | Likely tractable | Education + tooling |
| LeCun | Design (architecture choice) | Tractable | Open-weights + no restrictions |
| Brynjolfsson | Complementarity (design problem) | Implicit tractability | Human-complementary design |
| Acemoglu | Governance (institution design) | Depends on distribution | Labour policy + taxation |
| Bengio | Hard under agentic design, tractable under scientist AI | Conditional | Non-agentic constraints + intl coordination |
| Hinton | Control problem (possibly fundamental) | Uncertain / pessimistic | Binding international agreements |
| Marcus | Reliability first, then alignment | Reliability premature | FDA-style oversight + pause |

Notably: eight thinkers see alignment as tractable or resolvable through various paths. One (Hinton) is existentially concerned. One (Marcus) prioritises reliability over alignment framing.
