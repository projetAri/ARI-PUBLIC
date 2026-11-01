# ARI — Public Architecture v0.1

## Core flow

```mermaid
flowchart LR
    A[Event] --> B[Experience]
    B --> C[Memory]
    C --> D[Associations]
    D --> E[Hypothesis]
    E --> F[Test]
    F --> G[Evidence]
    G --> H{Validation}
    H -->|validated| I[Provisional Knowledge]
    H -->|conflict| J[Open Conflict / Abstain]
    I --> K[Action]
    K --> A
    J --> E
    I --> L[Revision]
    L --> C
```

## Governed knowledge lifecycle

```mermaid
flowchart TD
    M[Memory] --> A[Authority]
    A --> L[Lineage]
    L --> C[Context]
    C --> D[Dependencies]
    D --> R[Association]
    R --> H[Hypothesis]
    H --> T[Test]
    T --> E[Evidence]
    E --> V[Validation]
    V --> K[Provisional Knowledge]
    K --> X[Revision]
    X --> M
```

## Conflict behavior

```text
Equal contradictory authority  -> OPEN_CONFLICT / ABSTAIN
Stronger validated authority    -> SUPERSEDE, preserving lineage
Weaker incoming evidence        -> KEEP_CURRENT_AUTHORITY, preserve evidence
```

## Design objective

ARI's memory layer should eventually represent each meaningful relationship with:

```text
Relation
├── type
├── source / provenance
├── created_at
├── supporting_experiences[]
├── confidence
├── authority
├── validation_state
├── dependencies[]
├── contradictions[]
└── supersession_history[]
```

This document is conceptual. It is not a description of the private ALPHA implementation.
