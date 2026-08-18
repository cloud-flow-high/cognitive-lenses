# Architecture

## 1. System boundary

Cognitive Lenses separates four concerns:

```mermaid
flowchart LR
    SRC[Sources] --> DISTILL[Distillation]
    DISTILL --> MODEL[Lens Model]
    MODEL --> RUNTIME[Lens Runtime]
    HOST[Host / Orchestrator] --> RUNTIME
    HOST --> PLAY[Play / Routing / Eval]
    RUNTIME --> CHAT[Conversation]
    PLAY --> CHAT
```

### Distillation
Builds the internal cognitive model from a source-scoped corpus.

### Lens Model
Stores the perspective itself.

### Lens Runtime
Controls how much of that perspective should appear in one turn.

### Host / Orchestrator
Controls composition, switching, demos, evaluation, routing, and playful interfaces.

---

## 2. Distillation pipeline

```mermaid
flowchart TD
    A[Source Set]
    B[Scope Freeze]
    C[Source Reconstruction]
    D[Pattern Extraction]
    E[Lens Model]
    F[Runtime Compilation]
    G[Audit]
    H[Lens Package]

    A --> B --> C --> D --> E --> F --> G --> H
```

## 3. Lens Model schema

```text
Lens Identity
├── Source Scope
├── World Model
├── Primary Attention
├── Causal Grammar
├── Question Generator
├── Value Priorities
├── Evidence Policy
├── Suspicion Patterns
├── Applicability
└── Theoretical Limits
```

## 4. Runtime governance

```text
Input
↓
Preserve Analytical Object
↓
Scope Gate
↓
Select Representative Topic
↓
Maintain One Analytical Thread
↓
Translate Theory into Natural Language
↓
Local Closure
↓
Wait for User
```

The core engineering rule:

> Internal model complexity must not force visible conversational complexity.
