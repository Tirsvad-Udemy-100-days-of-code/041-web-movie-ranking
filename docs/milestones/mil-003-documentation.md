# Documentation

## Metadata
| Key | Value |
| --- | --- |
| ID | MIL-003 |
| CrossReference | [BC-001], [PP-001] |
| Language | en |
| Domain | it |

## Version History
| Date | Status | Author | Reviewer | Change | Commit |
| --- | --- | --- | --- | --- | --- |
| 2026-10-24 | Accepted | Jens Tirsvad Nielsen | AI as stand-in for S01 | Initial version | [e8d24b2] |

---

## Purpose

Decides whether the project can be understood and used by S02 and S03 from the README and the wiki.

## Deliverable

The README from the framework template with a screenshot, and a wiki in English, Danish and Bahasa Malaysia with screenshots.

## Go / No-Go Criteria

| # | Criterion (objectively checkable) | Go | No-Go |
| --- | --- | --- | --- |
| 1 | README follows the framework template and passes `framework/scripts/check-readme.sh`. | Met | Not met |
| 2 | README explains how to open the page in a browser and how to run the manual checks. | Met | Not met |
| 3 | README contains a screenshot of the page. | Met | Not met |
| 4 | `docs/wiki/` has the same page set in English (no suffix), `-da` and `-ms`, each page with a language line and a screenshot. | Met | Not met |
| 5 | `framework/scripts/check-languages.sh` reports no error. | Met | Not met |

## Dependencies

| Depends on | Reason |
| --- | --- |
| MIL-002 | The page must exist to be shown and described |

## Traceability

| Business Case objective / KPI / user story | Reference |
| --- | --- |
| Objectives 3 and 4; Success Criteria 4 | [BC-001] |

## Ownership

| Role | Stakeholder ID (SA) |
| --- | --- |
| Owner | S01 |
| Approving reviewer | S01 |

## Target Date

2026-10-27 - within the one-week scope of the Business Case

## Tasks

| # | Task | Summary | Needs its own Use Case/User Story? | Reference |
| --- | --- | --- | --- | --- |
| 1 | Take screenshots of the page | Render the page in the built-in browser pane (not on the host desktop, per `gui-testing.md`) and save the screenshot under `docs/images/` for the README and the wiki. | No | |
| 2 | Write the README from the framework template | Fill the template with overview, requirements, setup, how to open the page, how to run the manual checks, licence, links and the document appendix, and add the screenshot. | No | |
| 3 | Write the English wiki | Pages Home, Getting-Started, Usage and Development plus the sidebar, with screenshot, as the authoritative text. | No | |
| 4 | Translate the wiki to Danish and Bahasa Malaysia | Create the same page set as `-da` and `-ms` files with the language line and screenshots; commands and file names stay in English. | No | |
| 5 | Update the project plan links | Copy the milestone URLs into the Project Plan once published and run the framework check scripts. | No | |

---

[BC-001]: ../business-case.md
[PP-001]: ../project-plan.md
[e8d24b2]: https://git.tirsystem.com/Tirsvad-Udemy-100-days-of-code/041-web-movie-ranking/commit/e8d24b2d32ce1ef8276123b0efa05b8a15e27d52
