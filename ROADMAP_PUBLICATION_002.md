# ARI — Public Roadmap toward Publication 002

## Objective

Publication 002 should demonstrate a measurable mechanism that differentiates ARI from a document-centric retrieval system.

# ARI Associative Memory (AAM)

A governed memory layer in which relationships between experiences and concepts can be proposed, weighted, challenged, validated, superseded, and traced.

## Candidate public objects

- `Experience`
- `Memory`
- `Concept`
- `Relation`
- `Hypothesis`
- `Evidence`
- `Conflict`
- `Rule`
- `Decision`
- `Revision`

## Candidate relation metadata

- relation type
- provenance
- timestamps
- supporting experiences
- confidence
- authority level
- validation state
- dependencies
- contradictions
- supersession history

## M9 research objective

> Can ARI generate, preserve, test, and revise associations between memories while retaining full lineage and deterministic conflict handling?

## Minimum experimental set before Publication 002

- **EXP-AAM-01 — Association creation:** create a candidate relation without making it authoritative.
- **EXP-AAM-02 — Reinforcement:** independent evidence strengthens an association.
- **EXP-AAM-03 — Contradiction:** contradictory evidence preserves lineage and uncertainty.
- **EXP-AAM-04 — Authority resolution:** deterministic resolution across unequal authority.
- **EXP-AAM-05 — Equal-authority conflict:** verify `OPEN_CONFLICT / ABSTAIN`.
- **EXP-AAM-06 — Supersession:** replace an authoritative relation without erasing history.
- **EXP-AAM-07 — Reuse:** validated association influences a later hypothesis or decision.
- **EXP-AAM-08 — Rollback / reproducibility:** frozen-state replay yields the same governed result.

## Publication gate

Do not publish Publication 002 until:
- all core AAM tests pass;
- results are reproducible;
- a frozen public-safe result set exists;
- private implementation details have been reviewed;
- claims remain narrower than the evidence;
- comparisons with relevant approaches are documented.

## Proposed title

**ARI Associative Memory — A Governed Framework for Forming and Revising Relationships from Experience**

## Differentiation target

Publication 002 should make clear that ARI is not merely a RAG pipeline, vector store, static ontology, generic knowledge graph, or chat-history memory layer.

The differentiating mechanism should be experimentally visible:

**experience → association → hypothesis → evidence → conflict/validation → revision → reusable knowledge**
