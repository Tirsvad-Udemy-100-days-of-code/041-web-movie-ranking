# Movie page

## Metadata
| Key | Value |
| --- | --- |
| ID | MIL-002 |
| CrossReference | [BC-001], [PP-001] |
| Language | en |
| Domain | it |

## Version History
| Date | Status | Author | Reviewer | Change | Commit |
| --- | --- | --- | --- | --- | --- |
| 2026-10-24 | Accepted | Jens Tirsvad Nielsen | AI as stand-in for S01 | Initial version | [e8d24b2] |

---

## Purpose

Decides whether the Favorite Movie page meets the assignment and passes its manual checks.

## Deliverable

`src/index.html` and `src/styles.css`: the h1 "The Best Movies According to Tirsvad", the h2 "My top 3 movies of all-time.", an hr, and three h3 movies (13 element, 5th element, Drive) each followed by a p reason; and `tests/manual-checklist.md`, filled in.

## Go / No-Go Criteria

| # | Criterion (objectively checkable) | Go | No-Go |
| --- | --- | --- | --- |
| 1 | The page has exactly one h1 whose text is "The Best Movies According to Tirsvad", one h2 and one hr. | Met | Not met |
| 2 | The page has three h3 in the order 13 element, 5th element, Drive, each directly followed by a p. | Met | Not met |
| 3 | The page is valid HTML5 with `lang`, `charset` and `viewport`, and makes no external request. | Met | Not met |
| 4 | Every item of `tests/manual-checklist.md` is marked pass, checked in the browser pane. | Met | Not met |
| 5 | The page is reviewed against the assignment and the checklist with a `Go` record. | Met | Not met |

## Dependencies

| Depends on | Reason |
| --- | --- |
| MIL-001 | The skeleton must exist first |

## Traceability

| Business Case objective / KPI / user story | Reference |
| --- | --- |
| Objectives 1 and 2; Success Criteria 1, 2, 3 | [BC-001] |

## Ownership

| Role | Stakeholder ID (SA) |
| --- | --- |
| Owner | S01 |
| Approving reviewer | S01 |

## Target Date

2026-10-26 - within the one-week scope of the Business Case

## Tasks

| # | Task | Summary | Needs its own Use Case/User Story? | Reference |
| --- | --- | --- | --- | --- |
| 1 | Write index.html | Create the page from the HTML supplied by S01: the h1 "The Best Movies According to Tirsvad", the h2 "My top 3 movies of all-time.", an hr, and three h3 movies each followed by a p. Plain semantic HTML5, no script and no external request. | No | |
| 2 | Add styles.css | Add a small stylesheet for readable typography and spacing, linked from the page, so the page looks good without any dependency. | No | |
| 3 | Write and run the manual test checklist | Write `tests/manual-checklist.md` with one item per structural requirement and run it in the built-in browser pane (never on the host desktop), marking each item. | No | |
| 4 | Review the page against the assignment | Compare the page with the assignment and the checklist and record the result as an RC before the pull request. | No | |

---

[BC-001]: ../business-case.md
[PP-001]: ../project-plan.md
[e8d24b2]: https://git.tirsystem.com/Tirsvad-Udemy-100-days-of-code/041-web-movie-ranking/commit/e8d24b2d32ce1ef8276123b0efa05b8a15e27d52
