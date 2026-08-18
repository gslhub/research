# GSLHub Studies

This directory is reserved for public, study-level research documentation.

Each study should normally live in its own directory and include enough information to understand what was tested, how it was tested and which outputs are considered part of the release.

## Recommended study structure

```text
studies/<study-id>/
├── README.md
├── protocol.md
├── methodology.md
├── limitations.md
├── CHANGELOG.md
└── references.md
```

Datasets and executable software should normally live in their dedicated GSLHub repositories and be linked from the study README rather than duplicated.

## Study README checklist

A public study README should identify:

- study title and stable identifier;
- research question / hypothesis;
- authors and contributors;
- status and version;
- study period;
- systems and conditions evaluated;
- protocol version;
- primary metrics;
- dataset/output locations;
- known limitations;
- license and citation information;
- related publications or preprints.

## Release states

Suggested public states:

- `proposed` — design is visible but not frozen;
- `preregistered` — protocol frozen before data collection, when applicable;
- `collecting` — controlled data collection in progress;
- `analysis` — collection closed and analysis underway;
- `released` — public research output available;
- `archived` — historical study retained for reproducibility.

Internal application statuses may be more granular; this public vocabulary is intended for clear external communication.
