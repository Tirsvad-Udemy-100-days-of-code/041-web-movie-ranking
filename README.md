# 🚀 041 Web Movie Ranking

My solution to Day 41 of Udemy's "100 Days of Code: The Complete Python Pro Bootcamp": a plain HTML page that ranks my top 3 movies of all time. It is for fellow course participants and for anyone who browses the repository for ideas.

![The Best Movies According to Tirsvad][screenshot]

## 📚 Table of Contents

- [Overview](#-overview)
- [Requirements](#-requirements)
- [Setup](#-setup)
- [Run](#-run)
- [Tests](#-tests)
- [License](#-license)
- [Links](#-links)
- [Appendix: Project documents](#-appendix-project-documents)

## 🧭 Overview

"The Favorite Movie Project" asks for a web page with a title (`h1`), a subtitle (`h2`), a horizontal rule (`hr`), and at least three movies, each as an `h3` followed by a `p` that says why it is a favourite. This page has the title "The Best Movies According to Tirsvad" and ranks 13 element, 5th element and Drive.

The repository holds only HTML and CSS, with no dependencies:

- `src/index.html`: the page.
- `src/styles.css`: the typography and spacing.
- `tests/manual-checklist.md`: the checks that prove the page structure.
- `docs/`: the project documents and the wiki (English, Danish and Bahasa Malaysia).

## 📋 Requirements

A web browser. Nothing else is needed: there is no build step, no package to install and no server.

## 🛠️ Setup

Clone the repository:

```bash
git clone https://git.tirsystem.com/Tirsvad-Udemy-100-days-of-code/041-web-movie-ranking.git
cd 041-web-movie-ranking
```

## ▶️ Run

Open `src/index.html` in a browser by double-clicking it, or from a terminal:

```bash
# Windows
start src/index.html
# macOS
open src/index.html
# Linux
xdg-open src/index.html
```

## 🧪 Tests

The tests are a manual checklist, because the whole product is one static page. Open `src/index.html`, then go through the items of [`tests/manual-checklist.md`](./tests/manual-checklist.md) (one `h1`, one `h2`, one `hr`, three `h3` each followed by a `p`, no external request, and a narrow window without sideways scroll).

## 📄 License

[GNU Affero General Public License v3.0][license].

## 🔗 Links

- [Repository][repository]
- [Documentation][documentation]
- [Issue tracker][issues]

## 📎 Appendix: Project documents

The documents a newcomer needs, in reading order.

| Document | What it tells you |
| --- | --- |
| [AGENTS.md][agents] | The rules AI agents follow in this repository |
| [Business Case][BC-001] | Why the project exists, its scope and success criteria |
| [Stakeholder Analysis][SA-001] | Who is involved; the stakeholder IDs used for owners and reviewers |
| [Project Plan][PP-001] | The gateways and their schedule |
| [Milestones][milestones] | One document per gateway: Go/No-Go criteria and tasks |
| [Artifact registry][registry] | Where each artifact type lives, the next version, the PO language and domain |
| [Traceability matrix][TM-001] | How the artifacts link and when each was last reviewed |
| [Framework README][framework-readme] | The framework this project uses |
| [Framework changelog][framework-changelog] | What changed in each framework release |

The workflows installed from `TirSystem/github-action` need these secrets in the organisation: `TOKEN_FOR_GITEA` (publish accepted milestones) and `TOKEN_FOR_GITEA_WIKI` (publish the wiki, which must be enabled in the repository settings).

---

[screenshot]: ./docs/images/favorite-movie-page.jpg
[license]: ./LICENSE
[repository]: https://git.tirsystem.com/Tirsvad-Udemy-100-days-of-code/041-web-movie-ranking
[documentation]: https://git.tirsystem.com/Tirsvad-Udemy-100-days-of-code/041-web-movie-ranking/wiki
[issues]: https://git.tirsystem.com/Tirsvad-Udemy-100-days-of-code/041-web-movie-ranking/issues
[agents]: ./AGENTS.md
[BC-001]: ./docs/business-case.md
[SA-001]: ./docs/stakeholder-analysis.md
[PP-001]: ./docs/project-plan.md
[milestones]: ./docs/milestones/
[registry]: ./docs/artifact-registry.md
[TM-001]: ./docs/sqa/traceability-matrix.md
[framework-readme]: ./framework/README.md
[framework-changelog]: ./framework/CHANGELOG.md
