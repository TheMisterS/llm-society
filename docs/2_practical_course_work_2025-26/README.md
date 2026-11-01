# Practical course work (2025–2026)

**Visuomenės simuliacijos naudojant LLM** — *Simulating society with LLMs*
Kursinis projektinis darbas · Vilnius University, MIF · Supervisor: prof. dr. Aistis Raudys · 2026

| File | Description |
|------|-------------|
| [paper.pdf](paper.pdf) | Course work project paper (Lithuanian, 49 pages) |
| [slides_lt.pdf](slides_lt.pdf) | Defence presentation (Lithuanian) |
| [illustrations/](illustrations/) | Discussion graph diagrams (`graph_v0.0.1.png` is the first version, `graph.png` the final one) |

## Summary

This work designs and builds a discussion simulation in which a small group of LLM agents debate
(LangGraph, local models served through Ollama). It looks at the technical decisions, the architecture
and the problems that came up along the way. The system was developed in three stages:

1. **Stage 1** (§4.2): a supervisor-led discussion between agents with roles and traits, using
   short-term memory.
2. **Stage 2** (§4.3): long-term memory summarisation, a voting phase and prompt-engineering work,
   plus an analysis of how the discussion relates to the vote.
3. **Stage 3** (§4.4): an LLM-as-a-judge module that scores the generated discussions against
   predefined criteria.

## Code

The code as submitted is in the **`practical-cw-final`** tag:

```bash
git checkout practical-cw-final
# discussion system: "course_work_project(LLM Society)/app/"
# LLM judge:         "course_work_project(LLM Society)/judge/"
```

Related branches: `first_stage` (end of stage 1) and
`third_stage_1st_scenario` / `third_stage_2nd_scenario` (stage 3).

The code was later extended for the bachelor thesis and now lives in [`app/`](../../app/) on `main`.
The judge module is no longer there.
