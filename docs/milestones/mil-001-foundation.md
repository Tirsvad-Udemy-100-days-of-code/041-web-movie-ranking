# Foundation

## Metadata
| Key | Value |
| --- | --- |
| ID | MIL-001 |
| CrossReference | [BC-001], [PP-001] |
| Language | en |
| Domain | it |

## Version History
| Date | Status | Author | Reviewer | Change | Commit |
| --- | --- | --- | --- | --- | --- |
| 2026-10-24 | Accepted | Jens Tirsvad Nielsen | AI as stand-in for S01 | Initial version | [e8d24b2] |

---

## Purpose

Decides whether the repository skeleton, installed workflows and repository presentation are in place so that the page can be built on top of them.

## Deliverable

The folder skeleton (`src/`, `tests/`, `docs/`), a general `.gitignore`, the installed workflows, and the repository description and topics on the git host.

## Go / No-Go Criteria

| # | Criterion (objectively checkable) | Go | No-Go |
| --- | --- | --- | --- |
| 1 | `src/` and `tests/` exist and `.gitignore` ignores `.env`. | Met | Not met |
| 2 | The repository holds no Python file and no Python configuration. | Met | Not met |
| 3 | The workflows english-comments, publish-wiki and sync-milestones are in `.gitea/workflows/`, pinned to a released tag. | Met | Not met |
| 4 | The repository has a description and at least five topics on the git host. | Met | Not met |

## Dependencies

| Depends on | Reason |
| --- | --- |
| none | First milestone |

## Traceability

| Business Case objective / KPI / user story | Reference |
| --- | --- |
| Objectives 4 and 5; Success Criteria 5 and 6 | [BC-001] |

## Ownership

| Role | Stakeholder ID (SA) |
| --- | --- |
| Owner | S01 |
| Approving reviewer | S01 |

## Target Date

2026-10-25 - within the one-week scope of the Business Case

## Tasks

| # | Task | Summary | Needs its own Use Case/User Story? | Reference |
| --- | --- | --- | --- | --- |
| 1 | Create the folder skeleton and .gitignore | Add `src/` and `tests/` with placeholder files and a general `.gitignore` that ignores `.env`, editor files and operating system files. The repository stays HTML only, as the Business Case requires. | No | |
| 2 | Install workflows from TirSystem/github-action | Add `.gitea/workflows/` callers for English comments, publish wiki and publish accepted milestones, pinned to a released tag. The Python and shell quality checks are left out because the repository has no such files. Document the secrets S01 must create in the organisation. | No | |
| 3 | Set repository description and topics | Use the Gitea API with the token from the untracked `.env` (never imported or tested by the project) to set a description and topics on the repository, so S03 can find and understand it. | No | |

---

[BC-001]: ../business-case.md
[PP-001]: ../project-plan.md
[e8d24b2]: https://git.tirsystem.com/Tirsvad-Udemy-100-days-of-code/041-web-movie-ranking/commit/e8d24b2d32ce1ef8276123b0efa05b8a15e27d52
