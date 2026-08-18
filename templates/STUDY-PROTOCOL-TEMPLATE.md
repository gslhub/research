# Study Protocol Template

> Copy this file into `protocols/` or the relevant `studies/<study-id>/` directory and replace all placeholders.

## Metadata

- **Study ID:** `<stable-id>`
- **Title:** `<study-title>`
- **Protocol version:** `0.1.0`
- **Status:** `proposed`
- **Date:** `YYYY-MM-DD`
- **Authors:** `<names>`

## 1. Research question

State the primary question in a form that can be operationalized.

## 2. Hypothesis

Define the testable expectation(s), including null/alternative framing where appropriate.

## 3. Scope

Define:

- unit of analysis;
- target/source/entity being measured;
- systems/providers included;
- languages, locations or account conditions;
- study period;
- explicit out-of-scope conditions.

## 4. Experimental conditions

Describe the controlled condition set and identify which variables must remain fixed.

## 5. Prompt / intervention

Document the exact prompt or intervention, including version and checksum/reference where appropriate.

## 6. AI-system profile

Record the required system and interface conditions, such as:

- provider/system;
- model or interface version if observable;
- access mode;
- account tier;
- locale/timezone/location;
- web/search settings;
- memory/custom instructions;
- browser/device conditions.

## 7. Sampling and repetitions

Define sample size, number of repetitions, ordering/randomization and independence requirements.

## 8. Execution procedure

Specify the step-by-step procedure from environment preparation through completion.

## 9. Artifact preservation

Define mandatory raw artifacts and metadata, including integrity requirements such as SHA-256 where used.

## 10. Inclusion criteria

List conditions required for an execution/observation to enter analysis.

## 11. Exclusion criteria

List material deviations or failures that exclude a record from the primary analysis.

Excluded records should normally remain preserved with an explicit reason.

## 12. Coding procedure

Reference the applicable codebook and define observation/citation extraction steps.

## 13. Metrics and analysis

List primary/secondary metrics, formula versions and planned analysis procedure.

## 14. Quality control

Define review, validation, adjudication and reliability procedures.

## 15. Deviations and amendments

Explain how protocol deviations will be recorded and when a new protocol version is required.

## 16. Ethics, privacy and legal constraints

Document relevant privacy, platform terms, third-party rights, sensitive data or ethical considerations.

## 17. Limitations

Pre-specify known limitations and sources of uncertainty.

## 18. Outputs

List planned outputs:

- dataset;
- benchmark;
- technical report/preprint/publication;
- code/software;
- public dashboard or derived metrics.

## 19. Licensing

State the license for each output category or link to its canonical license metadata.

## 20. Freeze decision

- **Frozen for data collection:** `yes / no`
- **Freeze date:** `YYYY-MM-DD`
- **Approved by:** `<name/role>`
- **Protocol SHA / commit:** `<git-sha>`
