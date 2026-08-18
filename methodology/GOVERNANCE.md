# Research Governance

This document defines the default governance principles for public GSLHub research materials.

## 1. Version before modification

A methodological object that has been frozen for execution must not be silently rewritten. Material changes require a new version.

This applies especially to:

- research protocols;
- prompts used in controlled experiments;
- AI-system profiles;
- metric definitions;
- codebooks;
- inclusion/exclusion criteria.

## 2. Preserve observed evidence

Captured responses, screenshots, citations and raw research artifacts must represent what was actually observed.

Do not silently:

- correct generated text;
- rewrite citations;
- replace a failed execution with a successful one;
- remove an inconvenient result;
- change the recorded execution environment after the fact.

Corrections and annotations belong in separate governed metadata.

## 3. Separate development from scientific evidence

Synthetic fixtures, TEST executions and software-regression records are engineering evidence, not scientific findings.

Before real research begins, the study must establish a clean methodological baseline and freeze the relevant protocol versions.

## 4. Record deviations

Any material deviation from protocol must be documented.

A failed or excluded execution should normally remain in the audit trail with:

- execution identifier;
- reason for exclusion;
- relevant evidence;
- decision date;
- reviewer or decision authority where applicable.

A replacement execution requires a new identifier and explicit justification.

## 5. Traceability

Where methodology requires it, a published metric or conclusion should remain traceable through the research chain:

```text
Result / Metric
→ Observation
→ Execution
→ Evidence
→ Preserved Research Artifact
```

## 6. Access control

Not every research record is necessarily public.

Restricted records can include:

- credentials and account metadata;
- sensitive operational infrastructure;
- private researcher information;
- unpublished study materials;
- evidence that cannot legally or ethically be redistributed.

Public dissemination should expose only information approved for release.

## 7. Review

Research objects should use explicit review states where appropriate, such as draft, under review, validated, rejected or archived.

Validation should mean that both the content and its provenance satisfy the relevant methodological rules — not merely that a field is populated.

## 8. Research vs. product claims

GSLHub software capabilities and research findings must be communicated separately.

A feature that can calculate a metric does not prove a scientific conclusion. A deterministic test fixture validates software behavior, not the empirical hypothesis under study.

## 9. Amendments

Changes to these governance principles should be versioned and recorded through normal Git history. Material changes should explain their methodological rationale.
