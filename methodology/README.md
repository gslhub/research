# GSLHub Methodology

This directory contains stable methodological and governance documents that apply across GSLHub research studies.

## Canonical documents

- [`PROJECT-MATRIX.md`](PROJECT-MATRIX.md) — conceptual and operational model connecting scientific questions, experiments, executions, evidence, observations, citations, metrics and reproducibility.
- [`GOVERNANCE.md`](GOVERNANCE.md) — research-record governance, lifecycle, review and integrity principles.
- [`REPRODUCIBILITY.md`](REPRODUCIBILITY.md) — reproducibility requirements for protocols, execution context, preserved artifacts and research outputs.

## Boundary with the software repository

Scientific methodology is maintained in **`gslhub/research`**.

Implementation details, deployment procedures, CMS architecture, operational runbooks and software-specific behavior belong in [`gslhub/website`](https://github.com/gslhub/website).

When an implementation detail changes without changing the research method, the methodological document should not be version-bumped unnecessarily. When the scientific method changes materially, the canonical document in this repository must be updated and versioned as appropriate.

## Licensing

Except where otherwise noted, original methodological documentation is licensed under **CC BY 4.0**. See [`../LICENSE`](../LICENSE), [`../NOTICE.md`](../NOTICE.md) and [`../LICENSING.md`](../LICENSING.md).
