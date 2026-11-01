# ARI — An Experience-Centric Architecture for Associative and Continual Artificial Intelligence

## Version 0.1 — Foundational Architecture

**Publication candidate — 2026-11-01**

### Abstract

Most knowledge-enabled AI systems focus on retrieving information, structuring documents, or exposing organizational context to agents. ARI explores a different center of gravity: **experience**.

The project investigates an architecture in which observations, memories, associations, hypotheses, tests, evidence, conflicts, authority, and revision form a governed learning loop. Instead of treating memory as a passive store, ARI aims to make the relationships between memories explicit, traceable, revisable, and progressively reusable.

The central research question is:

> Can an AI system construct useful, auditable knowledge by repeatedly transforming experience into associations, hypotheses, evidence, and governed revisions?

ARI does not claim general autonomous learning or artificial consciousness. Its present contribution is an experimental, deterministic and governed infrastructure for studying these mechanisms.

---

## 1. Motivation

A large class of current AI architectures can be summarized as:

**Data / Documents → Retrieval / Context → Model → Answer or Action**

This is useful, but it leaves a gap. A system may retrieve relevant information without possessing a durable representation of **why** one relationship is trusted, where it came from, what contradicted it, how it evolved, or which experiment validated it.

ARI begins from a different question:

**What if the core unit of learning were not the document, but the experience?**

An experience has context, provenance, an outcome, a degree of authority, possible contradictions, and potential consequences for future reasoning.

---

## 2. Foundational principle

ARI is designed around the following principle:

> **ARI should not merely accumulate information. It should construct, test, and revise relationships between information.**

This leads to a second principle:

> **Knowledge is provisional when its supporting evidence is provisional.**

A memory can therefore be preserved without automatically becoming authoritative knowledge.

---

## 3. Experience as a first-class object

ARI distinguishes several conceptual layers:

- **Event** — something observed or received.
- **Experience** — an event interpreted in context and stored with provenance.
- **Memory** — a persistent representation derived from experience.
- **Association** — a typed relationship between memories or concepts.
- **Hypothesis** — a proposed relation or rule not yet sufficiently validated.
- **Experiment/Test** — a procedure intended to produce evidence.
- **Evidence** — an observation relevant to a hypothesis or rule.
- **Conflict** — incompatible evidence or claims that cannot be silently merged.
- **Authority** — a governed estimate of which claim currently has precedence.
- **Knowledge** — a currently accepted, traceable and revisable conclusion.
- **Revision** — an explicit change to accepted knowledge based on new evidence.

---

## 4. Governed Learning Loop

The public conceptual loop is:

**Memory → Authority → Lineage → Context → Dependencies → Association → Hypothesis → Test → Evidence → Validation → Provisional Knowledge → Revision**

The loop is intentionally governed.

When contradictory claims have equal authority, the system should not fabricate certainty. The preferred behavior is:

**OPEN_CONFLICT / ABSTAIN**

When a stronger claim is established, the prior claim can be superseded while its history remains traceable.

When incoming evidence is weaker than the current authoritative claim, the system can preserve the evidence while keeping the current authority.

This allows ARI to treat contradiction as data rather than as an error to be hidden.

---

## 5. Associative memory

ARI's intended associative memory is not limited to semantic similarity.

A relationship may include, for example:

- relation type;
- source / provenance;
- creation date;
- supporting experiences;
- confidence;
- authority level;
- validation state;
- dependency links;
- contradictory links;
- supersession history.

The long-term goal is for ARI to propose new useful associations from accumulated experience while preserving human-governed validation for changes that affect trusted knowledge.

---

## 6. Why this differs from document-centric context systems

A document-centric system typically asks:

> Which documents are relevant to the current query?

ARI additionally asks:

> Which experiences support this relation?  
> What contradicts it?  
> Which conclusion is currently authoritative?  
> Has it been tested?  
> What changed since the previous conclusion?  
> Can the relationship itself be revised?

This is not a rejection of retrieval, vector databases, ontologies, knowledge graphs, or agent protocols. Those can be components of ARI. The distinction is architectural: **the evolution of relationships through experience is treated as a core process rather than an incidental feature.**

---

## 7. Evolving ontology under governance

A fixed ontology can become a constraint if every useful concept must be defined in advance.

ARI therefore investigates a governed evolutionary approach:

1. existing concepts structure current knowledge;
2. repeated experiences reveal possible new relations or concepts;
3. ARI may formulate a candidate;
4. the candidate remains a hypothesis;
5. evidence and validation determine whether it can enter the trusted model;
6. every accepted change retains lineage.

The ontology is therefore not intended to be uncontrolled or self-modifying. It is **revisable under explicit governance**.

---

## 8. Current experimental status

As of 2026-11-01, the private ARI ALPHA environment has reached the **M8 freeze**.

The validated historical state includes:

- production version **0.1.7**;
- **8/8** M8 freeze checks passing;
- validated snapshot `ALPHA_M8_VALIDATED`;
- a present Learning Loop module;
- preservation of the frozen M7 state;
- EXP-047 preserved as a **CLOSED_CONFIRMATORY_SUCCESS / L6** authoritative experiment.

The publication intentionally reports this milestone without releasing the private ALPHA database, source tree, snapshots, protected experiments, or internal operational implementation.

---

## 9. Research claims — intentionally limited

This document does **not** claim that ARI has achieved:

- artificial general intelligence;
- consciousness or subjective experience;
- unrestricted autonomous self-improvement;
- autonomous general-purpose continual learning;
- scientifically demonstrated superiority to existing memory architectures.

The current claim is narrower:

> ARI provides a governed experimental framework for studying how experiences can become traceable associations, hypotheses, evidence, conflicts, and revisable knowledge.

---

## 10. Next research direction

The next architectural focus is the formalization of an **ARI Associative Memory (AAM)** layer.

Candidate object families include:

`Experience`, `Memory`, `Concept`, `Relation`, `Rule`, `Hypothesis`, `Conflict`, `Evidence`, `Decision`, and `Revision`.

Candidate relationships will carry metadata such as provenance, time, confidence, authority, validation state, and lineage.

Future publications should evaluate the architecture with reproducible experiments and explicit baselines.

---

## 11. Reproducibility and publication strategy

ARI is published in layers.

**Public layer**
- conceptual architecture;
- research claims;
- diagrams;
- selected reproducible examples;
- publication history.

**Private research layer**
- ALPHA laboratory source;
- internal database and snapshots;
- protected experimental implementation;
- unreleased operational mechanisms.

This boundary is deliberate: the objective of Publication 001 is to establish the research direction and its chronology without prematurely exposing the full implementation.

---

## 12. Conclusion

ARI proposes a shift in emphasis:

**From information retrieval to experience transformation.**

The target loop is:

**Event → Experience → Memory → Associations → Hypothesis → Test → Evidence → Validation → Knowledge → Action → New Event**

The distinctive research objective is not simply to remember more. It is to study whether a system can maintain a durable and auditable history of **how relationships are formed, challenged, validated, superseded, and reused**.

That is the foundation of ARI.
