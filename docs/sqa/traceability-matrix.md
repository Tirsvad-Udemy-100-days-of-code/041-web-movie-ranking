# Traceability Matrix

## Metadata
| Key | Value |
| --- | --- |
| ID | TM-001 |
| CrossReference | [BC-001] |

## Version History
| Date | Status | Author | Reviewer | Change | Commit |
| --- | --- | --- | --- | --- | --- |
| 2026-10-24 | Deprecated | Jens Tirsvad Nielsen | AI as stand-in for S01 | Initial version | [e8d24b2] |
| 2026-10-24 | Accepted | Jens Tirsvad Nielsen | AI as stand-in for S01 | Added RC-006 for the MIL-002 deliverable | pending |

---

## Purpose

Tracks backward/forward links between artifact instances so that the Business Case's
cross-artifact traceability success criterion is measurable. A row is added or
updated whenever an artifact instance is created or reviewed.

## Traceability Table

| Artifact Instance | Type | Language | Domain | Upstream (Backward Link) | Downstream (Forward Link) | Last Reviewed (RC-ID) |
| --- | --- | --- | --- | --- | --- | --- |
| [BC-001] | BC | en | it | - | [SA-001], [PP-001] | [RC-001] |
| [SA-001] | SA | en | it | [BC-001] | [PP-001] | [RC-002] |
| [PP-001] | PP | en | it | [BC-001], [SA-001] | [MIL-001], [MIL-002], [MIL-003] | - |
| [MIL-001] | MIL | en | it | [BC-001], [PP-001] | [MIL-002] | [RC-003] |
| [MIL-002] | MIL | en | it | [BC-001], [PP-001] | [MIL-003] | [RC-004], [RC-006] |
| [MIL-003] | MIL | en | it | [BC-001], [PP-001] | - | [RC-005] |

## Coverage Notes

No use case, domain model or design artifact exists: the project is too small for them. `-` in Last Reviewed for PP-001 means the Project Plan has no checklist; S01 accepts it (the AI as stand-in). `-` in Upstream means foundational; `-` in Downstream means nothing is built on it yet.

---

[BC-001]: ../business-case.md
[SA-001]: ../stakeholder-analysis.md
[PP-001]: ../project-plan.md
[MIL-001]: ../milestones/mil-001-foundation.md
[MIL-002]: ../milestones/mil-002-movie-page.md
[MIL-003]: ../milestones/mil-003-documentation.md
[RC-001]: ./reviews/rc-001-business-case.md
[RC-002]: ./reviews/rc-002-stakeholder-analysis.md
[RC-003]: ./reviews/rc-003-mil-001-foundation.md
[RC-004]: ./reviews/rc-004-mil-002-movie-page.md
[RC-005]: ./reviews/rc-005-mil-003-documentation.md
[RC-006]: ./reviews/rc-006-movie-page.md
[e8d24b2]: https://git.tirsystem.com/Tirsvad-Udemy-100-days-of-code/041-web-movie-ranking/commit/e8d24b2d32ce1ef8276123b0efa05b8a15e27d52
