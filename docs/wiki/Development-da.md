[English](Development) · **Dansk** · [Bahasa Malaysia](Development-ms)

# Udvikling

## Mapper

| Mappe | Indhold |
| --- | --- |
| `src/` | `index.html` og `styles.css` |
| `tests/` | Den manuelle tjekliste |
| `docs/` | Business Case, interessentanalyse, projektplan, milepæle, gennemgangsnotater, billeder og denne wiki |
| `framework/` | SQA- og QC-rammeværket (et git-submodul, som ikke redigeres her) |

## Sådan foregår arbejdet

Projektet har tre milepæle: Foundation, Movie page og Documentation. Hver milepæl har sin egen gren og pull request, og hver opgave er en issue. En milepæl udgives til issue-systemet af et workflow, når dens dokument er godkendt med en `Go`-gennemgang.

## Workflows

Workflows kommer fra `TirSystem/github-action` (version `v2.2.0`):

| Workflow | Hvornår | Hvad det gør |
| --- | --- | --- |
| English comments | Pull request | Kontrollerer, at tilføjede kommentarer er på engelsk |
| Publish accepted milestones | Push til `main`, der ændrer milepæle eller gennemgange | Opretter milepæle og issues. Hemmelighed: `TOKEN_FOR_GITEA` |
| Publish wiki | Push til `main`, der ændrer `docs/wiki/` | Kopierer disse sider til wikien. Hemmelighed: `TOKEN_FOR_GITEA_WIKI` |

Python- og shell-kvalitetskontrollerne er ikke installeret, fordi repositoryet ikke har sådanne filer.

## Wikien

Wikien findes på engelsk, dansk og bahasa malaysia. Engelsk er den gældende tekst; de andre sprog følger den side for side (`Page.md`, `Page-da.md`, `Page-ms.md`).
