# ARI — Publication 001

**Version:** 0.1 — Foundational Architecture  
**Date:** 2026-11-01  
**Status:** Public draft / publication candidate

## What is ARI?

ARI is an experimental architecture centered on a simple idea:

> An intelligent system should not only accumulate information. It should build, test, trace, revise, and reuse relationships between information through experience.

ARI treats **experience** as a first-class object and organizes learning around traceable evidence, authority, conflicts, hypotheses, validation, and revision.

## Public scope

This repository/package intentionally documents the **conceptual architecture** and the **research direction** of ARI.

It does **not** disclose:
- the private ALPHA laboratory repository;
- production databases or snapshots;
- internal implementation details that are not required to understand the research contribution;
- protected experimental artifacts or private operational procedures.

## Current validated milestone

The private ALPHA branch reached **M8**, frozen on production version **0.1.7**, with:
- 8/8 M8 freeze checks passing;
- a validated snapshot `ALPHA_M8_VALIDATED`;
- a governed Learning Loop module;
- preserved prior M7 state;
- EXP-047 retained as an authoritative L6 confirmatory success.

These facts establish the historical state of the project; the public package does not expose the private implementation.

## Research direction

ARI explores an experience-centric loop:

**Event → Experience → Memory → Associations → Hypothesis → Test → Evidence → Validation → Knowledge → Action → New Event**

The intended long-term property is a memory whose **relationships can evolve under governance**, rather than a static store of retrieved documents.

## Documents

- `WHITEPAPER.md` — publication manuscript
- `ARCHITECTURE.md` — public architecture
- `DISCLOSURE_BOUNDARY.md` — what remains private
- `PUBLICATION_CHECKLIST.md` — release procedure
- `CITATION.cff` — citation metadata template
- `zenodo_metadata.json` — Zenodo metadata draft
- `COPYRIGHT_NOTICE.md` — copyright / licensing status

## Citation

Citation metadata is prepared in `CITATION.cff`. Creator names and final repository/DOI values must be filled in at publication time.
