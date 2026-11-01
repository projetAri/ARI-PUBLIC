# Publication 001 — Disclosure Boundary

## Public in v0.1

The following may be published:

- ARI research motivation;
- experience-centric architecture;
- public terminology;
- high-level Learning Loop;
- conflict/authority principles;
- high-level M8 milestone status;
- public diagrams;
- research limitations;
- future AAM direction.

## Keep private for Publication 001

Do **not** publish:

- the complete `PROJET ARI/ALPHA` working repository;
- production database contents;
- database snapshots;
- private backup trees;
- secret keys, tokens, credentials or machine-specific paths;
- internal scripts whose publication would disclose the complete mechanism;
- unreleased experiment payloads;
- full protected EXP-047 implementation or private evidence;
- private operational documentation;
- personal journal material not intended for scientific publication.

## Rule

Before any file is copied into `ARI-PUBLIC`, ask:

> Is this necessary for a third party to understand or reproduce the public claim?

If the answer is no, it stays private.

## Repository separation

Recommended structure:

```text
PROJET ARI/
├── ALPHA/                 # PRIVATE LAB
└── ARI-PUBLIC/            # PUBLICATION REPOSITORY
    ├── README.md
    ├── WHITEPAPER.md
    ├── ARCHITECTURE.md
    ├── CITATION.cff
    └── ...
```

Never initialize the existing private ALPHA folder as the public repository.
