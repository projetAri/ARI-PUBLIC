# ARI Publication 001 — Release Checklist

## A. Freeze the public content

- [ ] Review `WHITEPAPER.md`
- [ ] Review `ARCHITECTURE.md`
- [ ] Confirm that no ALPHA source code has been copied
- [ ] Confirm that no database, snapshot, credentials or personal material is present
- [ ] Choose the public creator/author names
- [ ] Decide the software/document license
- [ ] Add a public contact address only if desired

## B. Create the public repository

Suggested repository name:

`ARI-PUBLIC`

Suggested first tag:

`publication-001-v0.1`

Suggested release title:

`ARI Publication 001 — Foundational Architecture v0.1`

## C. Citation metadata

- [ ] Fill creator names in `CITATION.cff`
- [ ] Add final repository URL
- [ ] Add DOI after archiving
- [ ] Keep version `0.1`
- [ ] Keep release date `2026-11-01` only if publication occurs on that date; otherwise replace it with the actual public release date

## D. Archive / DOI

- [ ] Connect the public repository to an archival DOI service such as Zenodo
- [ ] Create the first public release
- [ ] Verify the archived record
- [ ] Record the DOI in `README.md`, `CITATION.cff`, and the project journal

## E. Historical record

After publication, record internally:

- release date;
- repository commit hash;
- release tag;
- DOI;
- exact public files;
- exact private M8 baseline from which Publication 001 was derived.

## F. Next publication

Publication 002 should only follow after reproducible experiments justify additional claims.
