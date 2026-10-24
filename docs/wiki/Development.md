**English** · [Dansk](Development-da) · [Bahasa Malaysia](Development-ms)

# Development

## Folders

| Folder | Content |
| --- | --- |
| `src/` | `index.html` and `styles.css` |
| `tests/` | The manual checklist |
| `docs/` | Business Case, Stakeholder Analysis, Project Plan, milestones, review records, images and this wiki |
| `framework/` | The SQA and QC framework (a git submodule, not edited here) |

## How the work is done

The project has three milestones: Foundation, Movie page and Documentation. Each milestone has its own branch and pull request, and each task is an issue. A milestone is published to the issue tracker by a workflow after its document is accepted with a `Go` review.

## Workflows

The workflows come from `TirSystem/github-action` (version `v2.2.0`):

| Workflow | When | What it does |
| --- | --- | --- |
| English comments | Pull request | Checks that added comments are English |
| Publish accepted milestones | Push to `main` that changes milestones or reviews | Creates milestones and issues. Secret: `TOKEN_FOR_GITEA` |
| Publish wiki | Push to `main` that changes `docs/wiki/` | Copies these pages to the wiki. Secret: `TOKEN_FOR_GITEA_WIKI` |

The Python and shell quality checks are not installed, because the repository has no such files.

## The wiki

The wiki is in English, Danish and Bahasa Malaysia. English is the authoritative text; the other languages follow it page by page (`Page.md`, `Page-da.md`, `Page-ms.md`).
