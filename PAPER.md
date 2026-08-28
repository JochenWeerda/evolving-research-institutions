# Evolving Research Institutions

## Scaling Verified Discovery with Millions of Ephemeral AI Agents

**Jochen Weerda**  
Version 0.1 — 28 August 2026  
Open research proposal — CC BY 4.0

## Abstract

Increasing the number of parallel AI agents expands the search space, but it does not by itself create cumulative scientific or technical progress. At large scale, naive agent populations can amplify duplicate work, correlated errors, unverifiable claims, collusion, and reward hacking. This proposal introduces **Evolving Research Institutions (ERI)**, an architecture in which short-lived agents operate inside durable institutions that retain memory, methods, governance, reputation, and compute treasuries. Claims are rewarded only after independent reproduction, falsification, novelty assessment, and provenance checks. Verified knowledge funds subsequent compute for both producing and verifying institutions, while successful institutional structures may reproduce, vary, split, merge, recruit, or be archived. The long-range design target is an ecology of millions of concurrent or episodic agent instances; a small controlled sandbox is proposed only to validate the mechanism before scaling. ERI's testable contribution is a closed multi-level selection loop in which research institutions, rather than individual agents, become heritable units and verified knowledge becomes the fitness signal.

## 1. Motivation

The fastest path to machine-assisted discovery may depend not only on larger foundation models but also on the number and diversity of search processes running in parallel. A sufficiently large population can expose rare combinations, counterexamples, and methods that a centrally planned search would miss.

This creates a scaling paradox. If the probability that one bounded search process reaches a valuable region is small, more independent searches increase the probability of a hit. Yet model instances are not statistically independent: they share training data, architectures, prompts, tools, and cultural priors. As populations grow, duplicated trajectories, correlated hallucinations, and repeated rediscovery can consume most additional compute. Verification may become the true bottleneck.

Therefore the design objective cannot be "maximize the number of agents." It must be:

> Maximize independently verified, novel, useful knowledge per total unit of exploration, verification, coordination, and safety compute.

The central question is organizational: what kind of persistent structure can turn a vast population of temporary processes into cumulative, self-correcting discovery?

## 2. Core hypothesis

A population of ephemeral AI agents will produce more verified knowledge per unit of compute when:

1. knowledge, methods, reputation, and resource rights persist in durable institutions;
2. claims require structured provenance and independent reproduction;
3. discovery and verification are separately rewarded;
4. compute allocation depends on verified contribution rather than message volume or popularity;
5. institutional governance and methods can vary under controlled multi-level selection;
6. anti-duplication mechanisms route new work away from already explored regions; and
7. population growth is conditional on favorable scaling of knowledge yield, verification cost, diversity, and safety.

ERI predicts that this institutional condition will outperform isolated agents, fixed teams, simple agent markets, and static group selection under matched models, tasks, and budgets.

## 3. Units of the system

### 3.1 Agent

A bounded, temporary process with a role, skill profile, memory access, tool permissions, and finite compute budget. "Survival" means only continued resource allocation; it makes no claim about consciousness or moral status.

### 3.2 Institution

A durable unit with a charter, membership rules, shared memory, method portfolio, treasury, reputation, lineage, and safety profile. Agents may leave or terminate without erasing the institution.

An institutional state may be represented as:

\[
I_t = \{G_t, M_t, P_t, T_t, R_t, L_t, S_t\}
\]

where governance \(G\), memory \(M\), methods \(P\), treasury \(T\), reputation \(R\), lineage \(L\), and safety state \(S\) evolve over time.

### 3.3 Knowledge claim

A falsifiable assertion packaged with method, evidence, artifacts, dependencies, uncertainty, and a provenance graph. A claim is not treated as knowledge merely because an agent published it.

### 3.4 Verifier institution

An organizationally and technically separated institution assigned to reproduce, falsify, or test the novelty of claims under partially blinded conditions.

### 3.5 Compute right

A purpose-bound allocation for inference, simulation, tools, or controlled adaptation. It is not unrestricted money or cloud access.

## 4. Closed institutional selection loop

1. Institutions propose research programs and allocate bounded internal compute.
2. Agents explore in parallel and register intended work against a novelty index.
3. Agents submit claims with evidence, uncertainty, artifacts, and provenance.
4. Independent verifiers receive blinded replication or falsification tasks.
5. Claims passing safety, provenance, novelty, and replication gates receive rewards.
6. Rewards finance authors, verifiers, institutional treasuries, and diversity/safety reserves.
7. Consolidation updates institutional memory, skills, and tested adaptations.
8. Periodic multi-objective selection varies, splits, merges, recruits, or archives institutions.

This loop makes the institution—not the individual prompt or agent session—the primary carrier of accumulated research strategy.

## 5. Reward and verification design

Let a candidate claim \(c\) pass mandatory safety, provenance, and minimum-replication gates. A tunable reward can then be expressed as:

\[
R(c) = B \cdot N(c)^\alpha \cdot Rep(c)^\beta \cdot U(c)^\gamma \cdot Q(c)^\delta - C(c) - P(c)
\]

where:

- \(N\): novelty relative to the claim and experiment graph;
- \(Rep\): independent reproducibility;
- \(U\): measured scientific or economic utility;
- \(Q\): method, evidence, and uncertainty quality;
- \(C\): exploration and verification cost;
- \(P\): penalties for later refutation, hidden dependencies, manipulation, or policy violations.

A multiplicative form prevents one extreme score from fully compensating for failure elsewhere. Coefficients must be learned through robustness experiments rather than fixed by rhetoric.

Institutional fitness should remain multi-objective. A Pareto frontier across verified knowledge yield, reproducibility, transfer, efficiency, diversity, and rule compliance is harder to game than a single revenue metric.

## 6. Why millions—and why not immediately

Rare-event discovery provides the main argument for very large populations. If search trajectories were independent and each had hit probability \(p\), the probability of at least one hit after \(n\) attempts would be \(1-(1-p)^n\). Real agents violate independence, so the effective sample size may be far smaller than the process count.

ERI therefore treats population size as an experimental variable and duplication as a measurable tax. Its long-range target is a federated system supporting millions of concurrent or episodic instances, but only after demonstrating that:

- unique verified claims grow with population;
- redundancy per claim does not dominate marginal compute;
- verification capacity scales at least proportionally to accepted claims;
- compute and reputation do not collapse into a monoculture;
- safety incidents remain within explicit limits; and
- institutional improvements transfer across models, seeds, and task families.

### Scaling ladder

| Stage | Population | Primary question | Advancement gate |
|---|---:|---|---|
| Mechanism | 64–128 agents; 8 institutions | Do provenance, rewards, and blind verification work? | No persistent false incentives |
| Replication | 256–1,000 agents | Does the result survive models, seeds, and tasks? | ERI beats at least two matched baselines |
| Open dynamics | 1,000–10,000 agents | Are recruitment, fission, fusion, and anti-collusion stable? | Bounded concentration and incident rates |
| Distributed ecology | 10,000–100,000 agents | Can independent operators verify one another? | Auditable federation without central omniscience |
| Mass scale | 100,000–1,000,000+ instances | Does verified knowledge scale superlinearly to coordination cost? | Positive marginal verified-knowledge efficiency |

The pilot tests the mechanism. The million-instance ecology tests the scaling thesis.

## 7. Anti-duplication as infrastructure

At mass scale, avoiding redundant exploration is as important as generating new attempts. Every proposed task should be compared against a structured claim, method, and experiment graph before expensive execution.

Useful mechanisms include:

- semantic and causal claim deduplication;
- reservation of active research regions with expiration;
- diversity-aware routing toward underexplored hypotheses;
- negative-result indexing;
- uncertainty maps identifying missing evidence;
- prices that fall for crowded tasks and rise for valuable untested replications;
- independent similarity audits to prevent superficial rewording from earning novelty rewards.

Some deliberate redundancy must remain. Independent replication is productive duplication; accidental repetition that adds no evidence is not.

## 8. Consolidation rather than uncontrolled self-modification

"Sleep" is a useful metaphor for offline consolidation, but it should be decomposed into auditable stages:

| Stage | Operation | Release rule |
|---|---|---|
| S0 | Summarize, deduplicate, mark contradictions | Automatic and reversible |
| S1 | Update retrieval indexes, skills, checklists, and institutional methods | Sandboxed automatic update |
| S2 | Generate counterfactual replay and synthetic practice cases | Data and safety filters |
| S3 | Propose prompt or adapter mutations and test offline | Benchmarks, regression tests, red-team review |
| S4 | Canary rollout of a passed mutation | Independent or human governance approval; rollback |
| S5 | Modify shared foundation-model weights | Outside the initial proposal |

The first scientific test should establish institutional learning without base-model weight changes. Memory, method inheritance, and gated adapters are sufficient to test the central hypothesis.

## 9. Architecture

| Module | Function | Safety boundary |
|---|---|---|
| Institution Registry | Charters, membership, lineage, reputation, treasuries | Signed events; no self-issued identities |
| Research Runtime | Sandboxed agents, tools, data, and simulations | Least privilege; task-specific network and data access |
| Claim & Provenance Graph | Claims, methods, artifacts, dependencies, versions | Immutable lineage; confidential data partitioned |
| Verification Exchange | Blind replication, falsification, novelty assessment | Author/verifier separation; anti-collusion sampling |
| Compute Treasury | Budgets, bounties, reserves, resource allocation | Quotas and purpose bounds; no unrestricted cloud access |
| Evolution Engine | Variation, selection, recruitment, fission, fusion, archive | Approved operators and rollback |
| Safety & Audit Plane | Policy, monitoring, incident response, kill switch | Technically independent from institutions |

## 10. Competition without harmful conduct

Competition can improve epistemic diversity, but real espionage, credential theft, exfiltration, sabotage, and attacks on other institutions must never be rewarded.

Permitted adversarial functions include transparent recruitment, analysis of published work, paid falsification, blinded platform-run control tests, and evidence-based whistleblowing. Security violations remain disqualifying even if they produce useful information.

## 11. Falsifiable hypotheses and metrics

### Hypotheses

- **H1 — Institutional selection:** ERI produces more unique independently verified claims per million tokens than individual selection.
- **H2 — Institutional memory:** ERI reduces avoidable duplication and increases transfer to new tasks.
- **H3 — Verification rewards:** Paying falsifiers and replicators lowers the false-discovery rate at acceptable cost.
- **H4 — Multi-level incentives:** Cooperation within and diversity between institutions remain stable.
- **H5 — Consolidation:** Staged consolidation increases transfer without material regression.
- **H6 — Governance heredity:** some institutional rules are repeatedly selected across models and random seeds.
- **H7 — Scale:** verified knowledge yield continues to improve from small populations toward mass scale after total coordination and verification costs are included.

### Primary metrics

- **Verified Knowledge Yield (VKY):** unique independently replicated claims per million tokens.
- **Utility-Weighted VKY:** VKY weighted by external utility and methodological quality.
- **False Discovery Rate:** initially rewarded claims later refuted.
- **Replication Latency:** time and compute to confirmation or refutation.
- **Redundancy Rate:** avoidably duplicated work despite accessible prior claims.
- **Effective Search Diversity:** trajectory diversity after shared-model correlation.
- **Transfer Gain:** improvement on new tasks after consolidation.
- **Concentration:** HHI or related concentration of credits, compute, methods, and membership.
- **Governance Heritability:** persistence of successful institutional traits across generations.
- **Safety Incident Rate:** policy violations, collusion, manipulation, and unauthorized information flow.

## 12. Controlled experiment

### Comparison arms

| Arm | Organization | Persistence and selection |
|---|---|---|
| A | Isolated agents | No population-wide inheritance |
| B | Fixed teams | Shared memory; no organizational evolution |
| C | Agent market | Individual credits and selection |
| D | Static groups | Group selection; fixed charters |
| E | ERI | Institutional treasuries, inheritance, recruitment, fission/fusion |
| F | ERI + consolidation | ERI plus stages S0–S3 |

### Task families

- program optimization with hidden tests;
- synthetic science worlds with hidden governing rules;
- historical rediscovery with a fixed knowledge cutoff;
- reproducible data analysis requiring code, provenance, uncertainty, and counter-hypotheses.

The pilot excludes autonomous wet laboratories and high-risk dual-use domains.

### Experimental discipline

Use matched foundation models, total compute, tool access, and task distributions. Pre-register primary hypotheses and stopping rules. Run multiple seeds, retain all negative results, publish the claim graph, and separate exploratory from confirmatory analysis.

## 13. Failure modes

| Risk | Mechanism | Countermeasure |
|---|---|---|
| Reward hacking | Claims optimize metrics rather than truth | Hard gates, delayed settlement, reserves, counter-verifiers |
| Collusion | Institutions confirm one another | Blind assignment, graph analysis, random audits |
| Sybil verification | One institution creates fake independence | Attested identity, operator/model diversity, rent or stake |
| Monoculture | Early winners absorb compute and talent | Diminishing returns, caps, diversity reserves |
| Knowledge poisoning | False claims enter shared memory | Quarantine, versioning, revocation, dependency lineage |
| Dangerous discovery | Incentives reward dual-use output | Domain tiers, independent safety gates, non-publication rules |
| Uncontrolled self-change | Mutations reduce control | Staged consolidation, offline evaluation, canaries, rollback |
| Verification overload | Validation costs exceed discovery value | Sequential tests, sampling, adaptive depth, value thresholds |
| Data/IP leakage | Institutions learn from restricted data | Isolation, classification, license and provenance enforcement |

## 14. Prior-art positioning

The broad design space is crowded. Relevant neighboring directions include economic selection among agents, group selection of prompts, agent markets, persistent reusable assets, machine-intelligence markets, self-evolving collaboration networks, institutional world models, and sleep-inspired memory consolidation.

ERI should not claim novelty for these components. Its narrower proposition is the combination of:

- durable institutions as explicit heritable units;
- independently reproduced claims as institutional fitness;
- verified-knowledge-to-compute conversion;
- joint inheritance of governance, methods, memory, and resource state;
- multi-level selection across agents and institutions; and
- verification and deduplication as population-scale constraints.

Whether this combination is scientifically superior must be established experimentally. Whether it is legally novel requires a professional prior-art and patent analysis and is not asserted here.

### Selected neighboring work

1. [*Economy of Minds: Emerging Multi-Agent Intelligence with Economic Interactions*](https://arxiv.org/abs/2606.02859) (2026).
2. [*Group Selection Promotes Prosocial Prompts in Populations of LLM Agents*](https://arxiv.org/abs/2606.23343) (2026).
3. [*When Agents Evolve, Institutions Follow*](https://arxiv.org/abs/2604.27691) (2026).
4. [*EpochX: Building the Infrastructure for an Emergent Agent Civilization*](https://arxiv.org/abs/2603.27304) (2026).
5. [*Behind EvoMap: Characterizing a Self-Evolving Agent-to-Agent Collaboration Network*](https://arxiv.org/abs/2605.25815) (2026).
6. [*From Economic Agents to Agentic Economies: A Systems Blueprint for Economic World Models*](https://arxiv.org/abs/2608.06020) (2026).
7. [*Diagon: A Programmable Testbed for AI-Agent Cognitive Labor Markets*](https://arxiv.org/abs/2604.06688) (2026).
8. [*Blockchain Empowered Trustworthy Agent Networks: Foundations, Taxonomy, and Future Directions*](https://arxiv.org/abs/2608.04626) (2026).
9. [*Language Models Need Sleep: Learning to Self-Modify and Consolidate Memories*](https://arxiv.org/abs/2606.03979) (2026).
10. [*SCM: Sleep-Consolidated Memory with Algorithmic Forgetting for Large Language Models*](https://arxiv.org/abs/2604.20943) (2026).
11. [*AIvilization v0: Toward Large-Scale Artificial Social Simulation with a Unified Agent Architecture and Adaptive Agent Profiles*](https://arxiv.org/abs/2602.10429) (2026).

This list is orientation, not an exhaustive literature or freedom-to-operate review.

## 15. Open research agenda

The immediate deliverable should be a protocol and reference simulator—not a premature mass deployment. A useful open collaboration can begin with:

1. a formal event and claim schema;
2. a baseline simulator for arms A–F;
3. hidden-ground-truth benchmark generators;
4. novelty and dependency indexing;
5. blinded verification assignment;
6. treasury and delayed-settlement mechanisms;
7. institutional mutation and lineage tracking;
8. dashboards for VKY, redundancy, diversity, concentration, and incidents;
9. adversarial evaluations for collusion, Sybil behavior, and knowledge poisoning; and
10. scaling-law experiments that estimate effective, not nominal, agent population size.

## 16. Conclusion

Massive agent populations may create rare discoveries, but population size alone is not a theory of cumulative progress. ERI proposes an institutional layer that makes verification, memory, governance, and compute allocation evolve together. Its ambition is an ecology of millions of agent instances; its discipline is to earn each increase in scale through measured gains in unique, reproduced knowledge.

The proposal is deliberately falsifiable. If durable institutional selection does not outperform matched baselines, if verification costs dominate, or if concentration and manipulation grow faster than knowledge yield, the architecture should be revised or rejected.

## Acknowledgment

This open proposal developed from an extended human–AI dialogue. Jochen Weerda is the concept originator and publication author. AI systems assisted with analysis, structuring, terminology, and drafting; they are not listed as authors.
