---
type: moc
title: Policy Positions on AI Governance
domain:
- policy
- governance
status: permanent
created: 2026-06-30
updated: 2026-07-08
topic:
- topic/governance
- topic/ai-policy
wiki_indexed: '2026-07-12T00:00:00Z'
wiki_hash: 0e62002275414aebcf50edcc516a648a58c259ad87283bd4a35d5190cbdad785
wiki_role: moc
---



# Policy Positions on AI Governance

A synthesis of thinker positions on how society should govern frontier AI: through top-down regulation, decentralised tooling and education, international coordination, or some combination. Covers the fundamental question: who decides what AI can do?

## 1. Regulation Advocates (Top-Down Policy / FDA-Style Oversight)

This camp favours binding rules, pre-deployment testing, and government authority to restrict high-risk uses.

**Dario Amodei** [[20_People/dario-amodei/profile|dario-amodei]]: Pro-regulation on frontier models; export controls on compute; RSPs (Responsible Scaling Policies) as voluntary floor, but he expects and supports regulatory ceilings above them. Supports compute export controls on advanced models. Advocates for government capacity building via AI Safety Institutes and mandatory pre-deployment testing. Key testimonies and essays: [[10_Sources/Media/dario-amodei/senate-testimony-2023|US Senate Testimony (2023)]], [[10_Sources/Articles/dario-amodei/policy-on-the-ai-exponential-2026|Policy on the AI Exponential (2026)]].

**Gary Marcus** [[20_People/gary-marcus/profile|gary-marcus]]: Strong pre-deployment regulation; support for FDA-style approval for high-stakes applications. Views Silicon Valley as resistant to regulation and thus advocates for government oversight analogous to drug or aviation approval. Key book: [[10_Sources/Books/gary-marcus/taming-silicon-valley-2024|Taming Silicon Valley: How We Can Ensure That AI Works for Us (2024)]]. Key testimony: [[10_Sources/Media/gary-marcus/senate-testimony-2023|Senate Testimony: Oversight of A.I. (2023)]].

**Geoffrey Hinton** [[20_People/geoffrey-hinton/profile|geoffrey-hinton]]: Supports binding international agreements on frontier AI. Compares AI governance to nuclear weapons governance: international agreements, inspections, enforcement. Implicit assumption: national regulation alone is insufficient; coordination prevents a race-to-the-bottom. Key talks: [[10_Sources/Media/geoffrey-hinton/mit-tech-review-2023|MIT Technology Review (2023)]], [[10_Sources/Media/geoffrey-hinton/on-point-2025|On Point (2025)]].

**Paul Christiano** [[20_People/paul-christiano/profile|paul-christiano]]: Evaluations first; compute-thresholds; dangerous-capability red-teaming. Framing: mandatory pre-deployment evals for frontier models; compute-thresholds trigger higher scrutiny; dangerous-capability discovery requires red-teaming *before* release. Head of AI Safety at US AISI; policy direction shaped by governance (not individual lab commitments). Key papers: [[10_Sources/Papers/paul-christiano/elk-2021|Eliciting Latent Knowledge (2021)]]. Policy position implicit in [[20_People/paul-christiano/profile|profile]].

**Yoshua Bengio** [[20_People/yoshua-bengio/profile|yoshua-bengio]]: International coordination; mandatory evaluations; precautionary principle. Lead author of the International AI Safety Report (2025). Framing: no single nation should dominate frontier AI; governance requires binding multilateral agreements; evaluate before deploying.

### Consensus within this camp

- Frontier AI poses risks high enough to warrant pre-deployment testing.
- Markets alone do not internalise safety externalities.
- Government has a role; whether as direct regulator (Marcus), standard-setter (Christiano), or international coordinator (Bengio, Hinton).
- Voluntary commitments (RSPs) are insufficient; legal enforcement necessary.

---

## 2. Bottom-Up Tooling and Education Advocates

This camp favours decentralised access, user education, and architectural openness over top-down rules.

**Andrej Karpathy** [[20_People/andrej-karpathy/profile|andrej-karpathy]]: Prefers bottom-up tooling and education over top-down rules. Founding thesis of Eureka Labs (AI-native education, 2024–2026): the bottleneck on adoption is education. Implicit framing: distribute power through capability, not restrict it through policy. Users and developers need to understand models (hence education) and have access to tools (open weights, open APIs). Key talks: [[10_Sources/Media/andrej-karpathy/llm-os-2023|LLM OS (2023)]], [[10_Sources/Articles/andrej-karpathy/power-to-the-people-2025|Power to the People: How LLMs Flip the Script on Technology Diffusion (2025)]].

**Yann LeCun** [[20_People/yann-lecun/profile|yann-lecun]]: Opposes restrictive frontier regulation; pro open-source weights. Framing: regulation gives incumbents competitive advantage; open-source decentralisation is inevitable and healthy. Government should not restrict AI research; competition and decentralisation are the best governance. Open-weights release (Llama 2023–2024) reflects this stance. [[20_People/yann-lecun/profile|Profile]].

### Consensus within this camp

- Information (education) and tools (open weights) distribute power more equitably than rules.
- Monopoly control by frontier labs is the real risk; regulation entrenches it.
- Users and developers should be trusted; restrictions are paternalistic.
- Markets and decentralisation are better governance than governments.

---

## 3. International Coordination Advocates

This camp emphasises multilateral agreements and cross-border governance, especially for frontier compute and evaluation standards.

**Dario Amodei**: Compute export controls as part of a multilateral regime. Supports US-UK-allied coordination but frames it as necessary because China will pursue AI without restrictions. Policy must be aligned internationally or fails.

**Geoffrey Hinton**: Binding international agreements on frontier AI. Nuclear analogy: inspection, enforcement, verification across borders. No nation-state can solve this alone.

**Yoshua Bengio**: International AI Safety Report (2025) as practical output. Coordination on evaluations, thresholds, and precaution. Prefers binding agreements over voluntary commitments.

**Paul Christiano**: Compute-thresholds as a coordination mechanism. If major labs and governments agree that models beyond X compute trigger mandatory evaluations, this buys time for safety research across jurisdictions.

### Consensus within this camp

- Frontier AI is a global coordination problem.
- Voluntary lab commitments (RSPs) are good but insufficient.
- Export controls and compute thresholds can slow the race.
- Multilateral evaluation standards raise the floor for safety.

---

## 4. Tensions in Policy Thinking

### Regulation vs. innovation

**Amodei & Marcus vs. LeCun**: Amodei and Marcus accept innovation slowdown as a price for safety. LeCun argues regulation kills innovation and entrenches incumbents. Unresolved: can we regulate safely without stalling beneficial research?

### National vs. international coordination

**Hinton & Bengio vs. Amodei**: Hinton and Bengio emphasise binding *international* agreements as essential. Amodei's compute-export-controls imply US-led governance, not truly multilateral. Unresolved: is US-allied coordination sufficient, or does China's non-participation doom it?

### Precaution vs. access

**Christiano (evaluations) vs. Karpathy (education)**: Christiano wants to gate deployment until evals pass. Karpathy wants to open weights and educate users. Can we do both? Or does gating delay adoption whilst open access enables rapid, uncontrolled deployment?

### Lab commitments vs. government policy

**Amodei (RSPs + regulatory floor) vs. LeCun (open source)**: Amodei sees voluntary lab commitments as a foundation for government regulation. LeCun sees them as theater that delays open-source inevitability. Unresolved: do RSPs build trust for regulation, or do they legitimise industry self-regulation?

---

## 5. Policy Sources and Testimony

### Regulation and safety-first positions

**Dario Amodei**:
- [[10_Sources/Media/dario-amodei/senate-testimony-2023|Written Testimony of Dario Amodei, Ph.D., Senate Judiciary Committee (2023)]]
- [[10_Sources/Articles/dario-amodei/policy-on-the-ai-exponential-2026|Policy on the AI Exponential (2026)]]
- [[10_Sources/Articles/dario-amodei/on-deepseek-and-export-controls-2025|On DeepSeek and Export Controls (2025)]]

**Gary Marcus**:
- [[10_Sources/Media/gary-marcus/senate-testimony-2023|Senate Testimony: Oversight of A.I. (2023)]]
- [[10_Sources/Books/gary-marcus/taming-silicon-valley-2024|Taming Silicon Valley (2024)]]
- [[10_Sources/Media/gary-marcus/ieee-spectrum-ais-leading-critic-2024|How and Why Gary Marcus Became AI's Leading Critic (2024)]]

**Geoffrey Hinton**:
- [[10_Sources/Media/geoffrey-hinton/on-point-2025|On Point: The Godfather of AI says we can't afford to get it wrong (2025)]]
- [[10_Sources/Media/geoffrey-hinton/nobel-interview-2024|Nobel Prize Interview (2024)]]
- [[10_Sources/Media/geoffrey-hinton/60-minutes-2023|60 Minutes: Promise and risks of advanced AI (2023)]]

**Paul Christiano**:
- [[10_Sources/Media/paul-christiano/dwarkesh-preventing-ai-takeover-2023|Paul Christiano: Preventing AI Takeover (2023)]]
- [[10_Sources/Papers/paul-christiano/elk-2021|Eliciting Latent Knowledge (2021)]]
- [[10_Sources/Articles/paul-christiano/what-failure-looks-like|What failure looks like]]

**Yoshua Bengio**:
- [[10_Sources/Papers/yoshua-bengio/international-ai-safety-report-2025|International AI Safety Report (2025)]]

### Open-source and innovation-first positions

**Andrej Karpathy**:
- [[10_Sources/Articles/andrej-karpathy/power-to-the-people-2025|Power to the People: How LLMs Flip the Script on Technology Diffusion (2025)]]
- [[10_Sources/Media/andrej-karpathy/llm-os-2023|LLM OS (2023)]]
- [[10_Sources/Articles/andrej-karpathy/software-2-0|Software 2.0 (2017)]]

**Yann LeCun**:
- [[20_People/yann-lecun/profile|Yann LeCun profile]] — Meta AI and open-weights strategy
- [[10_Sources/Papers/yann-lecun/path-towards-autonomous-machine-intelligence-2022|Path Towards Autonomous Machine Intelligence (2022)]]

---

## 6. Policy Spectrum (Mapped)

| **Thinker** | **Approach** | **Mechanism** | **Scope** |
|---|---|---|---|
| Marcus | Regulation | FDA-style pre-approval | Frontier + high-stakes |
| Amodei | Regulation + industry | Compute export controls + RSPs | Frontier models |
| Christiano | Governance (evals + thresholds) | Mandatory pre-deployment testing | Frontier + dangerous capabilities |
| Bengio | International coordination | Binding multilateral agreements | Frontier (global) |
| Hinton | International coordination | Treaties (nuclear analogy) | Frontier (global) |
| Karpathy | Bottom-up tooling + education | Open weights + user education | All AI, not just frontier |
| LeCun | Open-source + competition | Decentralisation + market forces | All AI; oppose restrictions |
| Acemoglu | Institutional (labour policy) | Taxation + labour institutions | AI-driven automation (macro) |
| Brynjolfsson | Design + complementarity | Human-complementary AI focus | Task-level AI design (micro) |

---

## 7. The Unresolved Policy Consensus

**On goals**: All thinkers want AI to benefit society and avoid catastrophic harms. Hinton and Bengio prioritise existential risk. Acemoglu prioritises distributional justice. LeCun prioritises innovation. Amodei and Christiano balance all three.

**On mechanisms**: The divide is sharp. Some believe government regulation and international treaties are essential. Others believe decentralisation and open-source are inevitable and preferable. A middle ground (Amodei's approach: industry RSPs as foundation for regulatory floors) is untested.

**On timing**: Regulation proponents (Marcus, Amodei, Christiano) argue we must act *before* capabilities cross dangerous thresholds. Open-source advocates (LeCun, Karpathy) argue restrictions are futile; decentralisation will happen anyway.

**The core unresolved question**: Can top-down governance stabilise frontier AI development? Or does decentralisation prevent any single regime from controlling AI?
