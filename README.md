<div align="center">

# GSLHub Research

### Generative Search · GEO · AI Evaluation · Reproducible Research

**Canonical protocols, methodology, codebooks and public study materials for GSLHub**

**English** · [Español](./README.es.md)

[Website](https://gslhub.com) · [Platform](https://github.com/gslhub/website) · [Benchmarks](https://github.com/gslhub/benchmarks) · [Software](https://github.com/gslhub/software) · [Organization](https://github.com/gslhub)

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)

</div>

---

## Purpose

This repository is the **canonical methodological research layer** of **GSLHub — Generative Search Lab Hub**.

GSLHub investigates how generative AI systems **discover, select, cite and recommend information**, with particular emphasis on **Generative Search** and **Generative Engine Optimization (GEO)**.

The repository separates scientific methodology from the application code that executes and governs the research workflow. Protocols, codebooks, methodological decisions and reproducibility materials can therefore be inspected, cited and versioned independently from the software platform.

## Canonical research model

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

See the canonical [`Project Matrix`](methodology/PROJECT-MATRIX.md).

## Current research focus

- **Generative Search** — how generative systems retrieve, synthesize and surface information.
- **Generative Engine Optimization (GEO)** — factors associated with source selection, citation and recommendation.
- **AI-system evaluation** — controlled comparison of model/interface behavior under recorded conditions.
- **Source visibility** — measurable inclusion, citation, position and consistency outcomes.
- **Evidence governance** — provenance between prompts, executions, artifacts, observations and metrics.
- **Reproducibility** — versioned protocols, environment snapshots, integrity checks and review procedures.

## Core metrics

| Code | Metric | Purpose |
|---|---|---|
| **AIR** | Answer Inclusion Rate | Frequency with which a defined target appears in eligible answers |
| **CR** | Citation Rate | Frequency with which a defined target is cited in eligible answers |
| **MCP** | Mean Citation Position | Mean visible citation position for eligible citations |
| **RCR** | Response Consistency Rate | Consistency across controlled repeated responses under the defined coding rule |

Metric definitions and individual results are versioned separately.

### Specification and implementation boundary

This repository defines the **research meaning, coding rules and protocol context**. The versioned normative benchmark specifications live in [`gslhub/benchmarks`](https://github.com/gslhub/benchmarks), while the reusable deterministic implementations live in [`gslhub/software`](https://github.com/gslhub/software).

The first reusable implementation, [`@gslhub/metrics-core`](https://github.com/gslhub/software/tree/main/packages/metrics-core), calculates AIR, CR, MCP and RCR independently of Payload CMS, MongoDB or Next.js. Its automated tests reproduce the synthetic validation fixture published by the benchmark repository; those fixture values are software-validation data, **not empirical research findings**.

This separation supports an auditable chain:

```text
research meaning / coding rules
→ benchmark specification
→ independent software implementation
→ governed platform integration
→ validated research result
```

## Canonical methodological materials

### Project model

- [`methodology/PROJECT-MATRIX.md`](methodology/PROJECT-MATRIX.md) — conceptual and operational model linking scientific problem, hypotheses, experiments, executions, evidence, observations, citations, metrics and reproducibility.

### First controlled GEO pilot

- [`protocols/GSL-GEO-BENCH-01/PILOT-PROTOCOL-v0.1.0-ES.md`](protocols/GSL-GEO-BENCH-01/PILOT-PROTOCOL-v0.1.0-ES.md) — five controlled independent repetitions, evidence preservation, execution-context capture, exclusion rules and metric calculation.

### Observation and citation codebook

- [`codebooks/OBSERVATIONS-CITATIONS-v0.1.0-ES.md`](codebooks/OBSERVATIONS-CITATIONS-v0.1.0-ES.md) — formal coding, review, inclusion, exclusion and validation rules for observations and citations.

## Repository structure

```text
research/
├── protocols/       # Versioned research and pilot protocols
├── studies/         # Public study definitions and study-level documentation
├── codebooks/       # Coding rules for observations, citations and evidence
├── methodology/     # Stable methodological principles and research governance
├── templates/       # Reusable study/protocol templates
├── CITATION.cff     # Repository citation metadata
├── LICENSE          # CC BY 4.0 legal code
├── NOTICE.md        # Copyright, attribution and exclusions
└── LICENSING.md     # Licensing model by research-output type
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

See [`methodology/REPRODUCIBILITY.md`](methodology/REPRODUCIBILITY.md) and [`methodology/GOVERNANCE.md`](methodology/GOVERNANCE.md).

## Licensing

Except where a file or output explicitly states otherwise, **original research documentation in this repository is licensed under CC BY 4.0**.

Datasets, publications, software, third-party materials and GSLHub brand assets may use different licenses or terms. See [`LICENSE`](LICENSE), [`NOTICE.md`](NOTICE.md) and [`LICENSING.md`](LICENSING.md).

## Citation

This repository includes [`CITATION.cff`](CITATION.cff). When a study or publication provides its own citation instructions, cite that specific output in addition to the repository where appropriate.

## Contact

Research collaboration and methodological questions: **research@gslhub.com**

---

© 2026 Eduardo Yauri · GSLHub — Generative Search Lab Hub
