# Stakeholder Analysis

## Metadata
| Key | Value |
| --- | --- |
| ID | SA-001 |
| CrossReference | [BC-001] |
| Language | en |
| Domain | it |

## Version History
| Date | Status | Author | Reviewer | Change | Commit |
| --- | --- | --- | --- | --- | --- |
| 2026-10-24 | Accepted | Jens Tirsvad Nielsen | AI as stand-in for S01 | Initial version | pending |

---

## Purpose

This analysis names the people who care about the project, so that owners and reviewers in the other documents use stable IDs. It uses the power/interest grid: high power and high interest means Manage Closely.

## Stakeholder Summary Table

| ID | Name | Role/Title | Organization | Power Level | Interest Level | Quadrant | Primary Concern (Business Language) |
| --- | --- | --- | --- | --- | --- | --- | --- |
| S01 | Jens Tirsvad Nielsen | Course participant, Product Owner, developer and reviewer | Tirsvad (personal) | HIGH | HIGH | Manage Closely | A correct, well documented portfolio solution of the Day 41 assignment |
| S02 | Udemy coursists | Fellow participants who share code and compare solutions | Udemy course community | LOW | HIGH | Keep Informed | Readable HTML with the assignment's elements, and instructions to open and check it |
| S03 | GitHub viewers | Visitors who browse the repository for ideas | Public | LOW | MEDIUM | Keep Informed | A clear repository description, topics and README, and no dependencies |

## Power/Interest Classification Rationale

- **Manage Closely (S01):** decides scope, reviews every artifact and merges.
- **Keep Informed (S02, S03):** cannot change the project, but their ability to understand and run it is the measure of its quality. S03 has a medium interest because they only browse.

## Primary Concerns and FURPS+ Mapping

| ID | Concern | FURPS+ attribute |
| --- | --- | --- |
| S01 | The page meets the assignment and is verified by tests | Functionality, Reliability |
| S01 | The process is traceable and reviewed | Supportability (+ Design constraint) |
| S02 | The assignment's elements and a page that opens as is | Usability, Functionality |
| S02 | README and wiki instructions in a language they read | Usability, Supportability |
| S03 | Description, topics, README, no dependencies | Usability, Implementation constraint |

## Communication Requirements

| ID | Channel | Frequency | Deliverable | Phase / Milestone |
| --- | --- | --- | --- | --- |
| S01 | Chat, pull requests | Once per milestone | Pull request with review records | every milestone |
| S02 | README, wiki | At release | Open and check instructions in en, da, ms | documentation milestone |
| S03 | Repository page | At release | Description, topics, README with screenshot | foundation and documentation milestones |

## Conflicting Interests and Mitigations

| Conflict | Stakeholders | Mitigation |
| --- | --- | --- |
| S02 wants the assignment's exact elements; S01 wants a personal title and ranking | S01, S02 | Keep every required element (h1, h2, hr, three h3 each with a p) and personalise only the wording |
| S03 wants no dependencies; the checks are manual | S01, S03 | There is no tooling to install; the page is plain HTML |

## Traceability Analysis

### Business Goal Alignment

| Stakeholder | Concern | Business Case objective |
| --- | --- | --- |
| S01 | Page meets the assignment, tested | [BC-001] objectives 1 and 2 |
| S02 | Readable HTML | [BC-001] objectives 1 and 3 |
| S03 | Clear repository presentation | [BC-001] objectives 3, 4 and 5 |

## Sign-Off

| Stakeholder | Decision | Date |
| --- | --- | --- |
| S01 | Pending review (AI as stand-in on acceptance in autonomous mode) | |

---

[BC-001]: ./business-case.md
