[English](Development) · [Dansk](Development-da) · **Bahasa Malaysia**

# Pembangunan

## Folder

| Folder | Kandungan |
| --- | --- |
| `src/` | `index.html` dan `styles.css` |
| `tests/` | Senarai semak manual |
| `docs/` | Kes Perniagaan, Analisis Pihak Berkepentingan, Pelan Projek, pencapaian, rekod semakan, imej dan wiki ini |
| `framework/` | Rangka kerja SQA dan QC (submodul git, tidak diubah di sini) |

## Cara kerja dijalankan

Projek ini mempunyai tiga pencapaian: Foundation, Movie page dan Documentation. Setiap pencapaian mempunyai cabang dan pull request sendiri, dan setiap tugas ialah satu issue. Sesuatu pencapaian diterbitkan ke penjejak isu oleh satu workflow selepas dokumennya diterima dengan semakan `Go`.

## Workflow

Workflow datang daripada `TirSystem/github-action` (versi `v2.2.0`):

| Workflow | Bila | Fungsi |
| --- | --- | --- |
| English comments | Pull request | Menyemak bahawa komen yang ditambah dalam bahasa Inggeris |
| Publish accepted milestones | Push ke `main` yang mengubah pencapaian atau semakan | Mencipta pencapaian dan issue. Rahsia: `TOKEN_FOR_GITEA` |
| Publish wiki | Push ke `main` yang mengubah `docs/wiki/` | Menyalin halaman ini ke wiki. Rahsia: `TOKEN_FOR_GITEA_WIKI` |

Semakan kualiti Python dan shell tidak dipasang kerana repositori ini tiada fail sedemikian.

## Wiki

Wiki ini dalam bahasa Inggeris, Denmark dan Bahasa Malaysia. Bahasa Inggeris ialah teks utama; bahasa lain mengikutinya halaman demi halaman (`Page.md`, `Page-da.md`, `Page-ms.md`).
