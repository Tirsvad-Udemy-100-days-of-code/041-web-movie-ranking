# Business Case

## Metadata
| Key | Value |
| --- | --- |
| ID | BC-001 |
| CrossReference | [SA-001] |
| Language | en |
| Domain | it |

## Version History
| Date | Status | Author | Reviewer | Change | Commit |
| --- | --- | --- | --- | --- | --- |
| 2026-10-24 | Accepted | Jens Tirsvad Nielsen | AI as stand-in for S01 | Initial version | [e8d24b2] |

---

## Executive Summary

Day 41 of the Udemy course "100 Days of Code: The Complete Python Pro Bootcamp" asks the participant to build "The Favorite Movie Project": a plain HTML page with a title, a subtitle, a horizontal rule and at least three ranked movies, each with a reason. This project delivers exactly that page, as HTML only, with a README and a wiki that explain it, so that the course participants and the repository visitors can open, read and compare a clean solution. It contains no Python code and no dependencies.

## Methodological and Standards Foundation

The project follows the SQA and QC framework mounted at `framework/` (Business Case, Stakeholder Analysis, Project Plan, milestones, tasks, deliverables, each step reviewed). Quality is judged against ISO/IEC 25010:2023 characteristics, as the QC checklists tag them. The page follows the HTML5 standard.

## Problem Statement

The course assignment is usually solved as a file in a zip. A bare file gives no explanation of its structure, no recorded check that the required elements (h1, h2, hr, three or more h3 with a p each) are present, and no documentation a fellow participant can follow.

## Business Opportunity

Treating the assignment as a small documented project turns it into a portfolio piece: it shows the page, how it is structured and how to check it. Other participants (S02) and repository visitors (S03) can learn from it.

## Objectives

1. Deliver the Favorite Movie page in HTML: the h1 title "The Best Movies According to Tirsvad", the h2 "My top 3 movies of all-time.", an hr, and three h3 movies each followed by a p reason: 13 element, 5th element and Drive.
2. Verify the page structure with a written manual test checklist.
3. Document how to open the page in a browser and how to run the checks.
4. Publish the repository with a description, topics, a README with screenshot and a wiki in English, Danish and Bahasa Malaysia.
5. Install the shared workflows of `TirSystem/github-action` that fit an HTML-only repository.

## Scope

### In Scope

- `src/index.html` and `src/styles.css`; a manual test checklist under `tests/`; documents under `docs/`.
- A general `.gitignore` that ignores `.env`.
- README from the framework template with a screenshot; wiki in en, da and ms with screenshots.
- Repository description and topics; the fitting workflows installed from `TirSystem/github-action`.

### Out of Scope

- Python code or tooling of any kind (no `pyproject.toml`, venv, pytest, `constants.py`, Doxygen), a web server, a database, JavaScript, or a dependency.
- The other days of the course.

## Expected Benefits

### Tangible Benefits

- A finished `index.html` that opens in any browser, and a checklist that proves its structure.
- A repository that other participants can clone and open in minutes.

### Intangible Benefits

- Practice in project discipline: plan, review, check, document.
- A readable reference for the course community.

## Strategic Alignment

The repository belongs to the organisation that collects the solutions to the course. This project keeps the same structure and quality bar as the sibling projects, so the collection stays consistent.

## Success Criteria

| # | Criterion | Target | Measure |
| --- | --- | --- | --- |
| 1 | Page structure | one h1 with the agreed title, one h2, one hr, at least 3 h3 each followed by a p | checklist items 1 to 5 pass in a browser |
| 2 | Manual checks | every item of `tests/manual-checklist.md` passes | checklist filled in and committed |
| 3 | Dependencies | none | `src/` holds only `index.html` and `styles.css`, with no external requests |
| 4 | Documentation | README and wiki in 3 languages, each with a screenshot | every wiki page exists in `en`, `da`, `ms` |
| 5 | Repository metadata | description and at least 5 topics set | read from the git host API |
| 6 | Workflows | English comments, wiki publishing and milestone publishing installed | files present in `.gitea/workflows/` |

## Risks

| Risk | Impact | Mitigation |
| --- | --- | --- |
| Translations to Danish and Bahasa Malaysia contain errors | Readers are misled or find the wiki poor | English is authoritative; keep pages short and simple; S01 reviews the Danish pages |
| Screenshot cannot be taken without using the host desktop | The README and wiki lack an image | Render the page in the built-in browser pane, never on the host desktop (`gui-testing.md`) |
| Workflow secrets or runner are missing on the git host | Installed workflows fail | The README lists the secrets; the workflows are installed, their secrets are S01's to create |
| Tokens leak into the repository | Credential exposure | `.env` is ignored by git and is never read or imported by the project |

## Assumptions

- S01 is Product Owner, developer and reviewer; in autonomous mode the AI stands in as reviewer and says so in each review record.
- The PO language is English and the domain is IT.
- S01's ranking is 1. 13 element, 2. 5th element, 3. Drive, with the reasons S01 supplied as ready-made HTML (S01's own text is used as given).
- The git host repository already exists at `Tirsvad-Udemy-100-days-of-code/041-web-movie-ranking`.
- A Gitea token is available in the untracked `.env` for personal use only.

## Constraints

- HTML only: no Python and no other programming language.
- Delivery within one week of 2026-10-24 (by 2026-10-31).
- Folder structure `src/`, `tests/`, `docs/`; one branch and pull request per milestone.
- The framework under `framework/` is not edited from this project.

## Cost–Benefit Assessment

| Costs | Benefits |
| --- | --- |
| A few hours of AI-assisted work and S01's review time; no licence or infrastructure cost beyond the existing git host | A documented reference solution and a consistent repository; qualitative, as this is a learning project |

## Stakeholders

| Stakeholder ID (SA) | Interest in this project |
| --- | --- |
| S01 | Owns the product, develops and reviews; wants a clean portfolio project |
| S02 | Wants readable, runnable code with the assignment's names, and instructions to open it |
| S03 | Wants a clear description, topics and README, and no dependencies |

## Recommendation

Proceed — the scope is small, the risks have mitigations and the result serves all three stakeholders.

---

[SA-001]: ./stakeholder-analysis.md
[e8d24b2]: https://git.tirsystem.com/Tirsvad-Udemy-100-days-of-code/041-web-movie-ranking/commit/e8d24b2d32ce1ef8276123b0efa05b8a15e27d52
