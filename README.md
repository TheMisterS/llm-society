# LLM Society

Simulating society and multi-agent discussions with large language models.

This repository collects three consecutive academic works by Simonas Jaunius Urbutis
(Vilnius University, Faculty of Mathematics and Informatics, Informatics programme),
supervised by prof. dr. Aistis Raudys. Each work builds on the previous one: a literature
review, then a working discussion-simulation system, then a RAG-based persona study on top of it.

| # | Work | Period | Paper | Slides | Code |
|---|------|--------|-------|--------|------|
| 1 | **Theoretical course work** — *Simulating society with LLMs* | Spring 2025 | [paper.pdf](docs/1_theoretical_course_work_2025/paper.pdf) | [slides_lt.pptx](docs/1_theoretical_course_work_2025/slides_lt.pptx) | — |
| 2 | **Practical course work (project)** — *Simulating society with LLMs* | Sep 2025 – Jan 2026 | [paper.pdf](docs/2_practical_course_work_2025-26/paper.pdf) | [slides_lt.pdf](docs/2_practical_course_work_2025-26/slides_lt.pdf) | tag [`practical-cw-final`](https://github.com/TheMisterS/course_work-LLM-Society-/tree/practical-cw-final) |
| 3 | **Bachelor thesis** — *LLM Society: RAG based persona creation and their impact in a multi-agent discussion system* | Feb – May 2026 | [paper.pdf](docs/3_bachelor_thesis_2026/paper.pdf) | [slides_lt.pdf](docs/3_bachelor_thesis_2026/slides_lt.pdf) | [`app/`](app/) on `main` · tag [`bachelor-final`](https://github.com/TheMisterS/course_work-LLM-Society-/tree/bachelor-final) |

All papers and slides are written in Lithuanian (the bachelor thesis has an English abstract).
Each `docs/` folder has its own README with a short summary.

## Repository layout

```
app/     discussion system + RAG persona pipeline + evaluation (bachelor thesis version)
docs/    papers, slides and illustrations, one folder per work
```

To run the system, see [`app/README.md`](app/README.md).

## Code history

The code grew continuously across works 2 and 3, so `main` only holds the latest (bachelor) version.
The state of the code at each submission is preserved as a git tag:

- **`practical-cw-final`** — discussion system with short/long-term memory, voting and the
  LLM-as-a-judge evaluation module (`judge/`, later removed).
- **`bachelor-final`** — the submitted bachelor thesis code (same as `app/` on `main` at the time).

Other branches kept for reference:

| Branch | What it is |
|--------|------------|
| `first_stage` | End of the first development stage of the practical course work (paper §4.2) |
| `third_stage_1st_scenario`, `third_stage_2nd_scenario` | Snapshots from the third stage of the practical course work (LLM judge, paper §4.4) |
| `failed_society_survey_test` | Abandoned early bachelor approach: building personas from European Social Survey (ESS 11, 2024) microdata and comparing their answers to real respondents |
| `bachelor_v0.0.1`, `dev/setup` | Already merged into `main` |
