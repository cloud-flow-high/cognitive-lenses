# Forking Guide

Forking is a first-class design goal.

A Cognitive Lens is an interpretation bound to a source scope **and** an activation policy. Two forks may share the same source material while differing in what they choose to make salient during conversation.

## Good fork reasons

- narrower source scope;
- different period of the same thinker;
- single-book specialization;
- alternate school branch;
- different Selective Activation policy;
- different runtime pacing;
- another AI platform;
- visual interface;
- host/orchestrator experiments;
- evaluator integration;
- translation.

## Required fork metadata

A public Lens fork should document:

```text
Lens Name:
Based On:
Source Scope:
Excluded Scope:
Activation Policy Changes:
Runtime Changes:
Known Differences from Upstream:
Version:
```

## What may legitimately differ

A fork may change:

### Source scope
What material is considered authoritative for the Lens.

### Lens Model
How recurring concepts, causal structures, questions, and evidence preferences are reconstructed.

### Selective Activation
Which nodes receive priority in ordinary conversation, what gets suppressed, and when broader activation is allowed.

### Runtime
How activated material is expressed, paced, and disclosed.

### Host behavior
How lenses are switched, stacked, compared, evaluated, or forged.

These layers should be documented separately when possible.

## Naming

Prefer names that reveal scope.

Good:
- `late-foucault-ethics-lens`
- `discipline-and-punish-lens`
- `classical-liberalism-lens`

Less useful:
- `better-foucault`
- `real-foucault`
- `ultimate-liberalism`

A Lens is not a claim of final doctrinal authority.

It is a source-scoped, activation-governed interpretation that should remain open to audit and fork.
