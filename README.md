<div align="center">

# GSLHub Research

### Generative Search · GEO · AI Evaluation · Reproducible Research

**Research protocols, methodological documentation and study materials for GSLHub**

[Website](https://gslhub.com) · [Research platform](https://github.com/gslhub/website) · [Organization](https://github.com/gslhub)

</div>

---

## Purpose

This repository is the methodological research layer of **GSLHub — Generative Search Lab Hub**.

GSLHub investigates how generative AI systems **discover, select, cite and recommend information**, with particular emphasis on **Generative Search** and **Generative Engine Optimization (GEO)**.

The repository is designed to make research protocols, study definitions, methodological decisions and reproducibility materials inspectable independently from the application code that executes and governs the research workflow.

## Research model

GSLHub follows a traceable chain:

```text
Scientific problem
→ Hypothesis
→ Experiment
→ Controlled execution
→ Preserved research artifact
→ Evidence
→ Observation
→ Citation / Metric
→ Reproducibility review
→ Public dissemination
```

A metric is not treated as an isolated number. Where methodology requires it, the result must remain traceable through governed observations and executions to preserved evidence.

## Current research focus

- **Generative Search** — how generative systems retrieve, synthesize and surface information.
- **Generative Engine Optimization (GEO)** — factors associated with source selection, citation and recommendation.
- **AI-system evaluation** — controlled comparison of model/interface behavior under recorded conditions.
- **Source visibility** — measurable inclusion, citation, position and consistency outcomes.
- **Evidence governance** — provenance between prompts, executions, artifacts, observations and metrics.
- **Reproducibility** — versioned protocols, environment snapshots, integrity checks and review procedures.

## Core metrics

The current GSLHub methodology includes four governed metric families:

| Code | Metric | Purpose |
|---|---|---|
| **AIR** | Answer Inclusion Rate | Frequency with which a defined target appears in eligible answers |
| **CR** | Citation Rate | Frequency with which a defined target is cited in eligible answers |
| **MCP** | Mean Citation Position | Mean visible citation position for eligible citations |
| **RCR** | Response Consistency Rate | Consistency across controlled repeated responses under the defined coding rule |

Metric definitions are versioned and validated separately from individual results.

## Repository structure

```text
research/
├── protocols/       # Versioned research and pilot protocols
├── studies/         # Public study definitions and study-level documentation
├── codebooks/       # Coding rules for observations, citations and evidence
├── methodology/     # Stable methodological principles and research governance
├── templates/       # Reusable study/protocol templates
└── LICENSING.md     # Licensing model for research outputs
```

## Development vs. research data

GSLHub deliberately separates **software-development validation** from **scientific data collection**.

```text
DEVELOPMENT
build → test → detect → correct → validate → clean

RESEARCH
freeze protocol → establish clean baseline → execute → preserve → validate → analyse → publish
```

Synthetic TEST records and deterministic software fixtures must never be presented as scientific findings.

## Reproducibility principles

GSLHub research is designed around:

- versioned protocols and metric definitions;
- controlled execution-environment snapshots;
- isolated sessions where required by protocol;
- preservation of raw outputs and visible interfaces;
- SHA-256 integrity checks for preserved artifacts;
- explicit inclusion/exclusion criteria;
- lifecycle sealing for governed records;
- persistent artifact storage and recovery verification;
- documented deviations rather than silent replacement;
- independent review where the study design requires it.

See [`methodology/REPRODUCIBILITY.md`](methodology/REPRODUCIBILITY.md).

## Research integrity

Research records should preserve what was actually observed. Responses, citations and evidence must not be silently corrected or rewritten after capture.

Methodological changes require versioning. Excluded or failed executions are retained with an explicit reason rather than deleted from the research history.

See [`methodology/GOVERNANCE.md`](methodology/GOVERNANCE.md).

## Status

This repository is being prepared as the public methodological companion to the GSLHub research platform. Research materials are opened progressively after methodological review and removal of restricted or operational information.

## Licensing

Software, research documentation, datasets, publications and brand assets do not necessarily share the same license. See [`LICENSING.md`](LICENSING.md) before reusing materials from this repository.

## Contact

Research collaboration and methodological questions: **research@gslhub.com**

---

© 2026 GSLHub / Eduardo Yauri
