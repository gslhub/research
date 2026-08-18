# Reproducibility Framework

GSLHub is designed to preserve enough methodological and execution context for controlled generative-search experiments to be audited and, where feasible, repeated.

## Reproducibility stack

The current framework combines:

```text
Versioned protocol
+ frozen experimental conditions
+ controlled execution snapshots
+ preserved raw artifacts
+ Evidence ↔ Artifact provenance
+ SHA-256 integrity checks
+ explicit inclusion/exclusion criteria
+ lifecycle sealing
+ quality control and review
+ persistent storage
+ restart/redeploy verification
+ recovery testing
+ development/research separation
```

## Execution context

A controlled execution should record the variables needed to interpret the result, including those required by the relevant protocol.

Depending on the study, this may include:

- AI system and provider;
- visible model/interface version;
- access mode and account tier;
- date and time;
- locale and timezone;
- declared location;
- web/search availability and mode;
- memory state;
- custom instructions;
- browser and version;
- device and viewport;
- whether the session was new and isolated;
- visible incidents or interface changes.

The study protocol determines which variables are mandatory and which are descriptive metadata.

## Session independence

Where the study requires independent repeated responses, each repetition must begin from a new session without uncontrolled conversational context.

Regeneration and follow-up prompts should not substitute for an independent repetition unless the protocol explicitly studies those behaviors.

## Artifact preservation

Raw research artifacts may include:

- response exports;
- screenshots;
- PDFs;
- structured JSON/HTML exports;
- source panels;
- other files required to preserve the observable result.

Where supported, preserved files receive a SHA-256 digest so later integrity checks can detect modification or corruption.

## Provenance

Artifacts should not exist as anonymous files. They should be associated with the execution that produced them and with the governed evidence/observation chain used for analysis.

## Failures and exclusions

A failed execution is part of the research history.

If an execution is excluded, retain the record and document the reason. Do not silently delete it or reuse the same repetition identifier for a replacement.

## Storage resilience

Research reproducibility also depends on operational preservation. GSLHub therefore treats persistent storage, restart/redeploy survival and recovery testing as part of the research-infrastructure quality model.

## Reproduction vs. replication

GSLHub distinguishes conceptually between:

- **reproduction** — repeating a procedure as closely as possible using the recorded conditions and materials;
- **replication** — independently testing the same or related hypothesis, potentially under a new sample, period, system or controlled condition.

Study documentation should state which objective applies.

## Public release

A public research release should contain enough non-restricted information to understand:

1. the research question;
2. the protocol version;
3. the relevant system/condition definitions;
4. inclusion and exclusion rules;
5. coding rules;
6. metric definitions;
7. known limitations;
8. the provenance level of the published outputs.
