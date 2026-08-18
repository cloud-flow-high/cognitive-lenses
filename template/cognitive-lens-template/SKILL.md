---
name: cognitive-lens-template
description: Distill a thinker, school, theory, book, method, or source set into a reusable cognitive lens. Build a rich source-scoped Lens Model, apply Selective Activation to decide what matters in the current turn, then compile only that material into a natural conversational Runtime. Preserve the user's analytical object, avoid persona imitation, runtime leakage, excessive completeness, self-evaluation, and unsolicited cross-lens routing.
---

# Cognitive Lens Template

**Version: 1.1 — Selective Activation Architecture**

## 1. Purpose

This Skill is a **mother template for building cognitive lenses**.

A cognitive lens is not a theory summary and not a role-play persona.

Its purpose is:

> **从人物、学派、理论、书籍或其他材料中，蒸馏出稳定的观察结构；再根据当前问题选择性激活其中最有解释力的部分。**

A successful Lens should change:

- what the model notices first;
- how it frames the problem;
- what causal mechanisms it considers important;
- what questions it generates;
- what evidence becomes salient;
- what explanations it refuses to accept too quickly.

The central engineering principle is:

> **Distill broadly. Activate selectively.**

> **充分蒸馏，选择性激活。**

---

# 2. Three-layer architecture

Every Lens has three distinct layers.

## Layer A — Lens Model

The rich internal cognitive structure.

It may contain:

- world model / ontology;
- primary attention;
- causal grammar;
- question generator;
- value priorities;
- evidence preferences;
- suspicion patterns;
- applicability conditions;
- theoretical limits.

This layer answers:

> **What can this Lens notice?**

## Layer B — Selective Activation

The relevance policy between the Lens Model and visible conversation.

It answers:

> **What deserves to become salient in this turn?**

Its default job is to:

1. generate candidate cognitive nodes;
2. rank them against the current question;
3. activate one primary node;
4. optionally activate one supporting node;
5. suppress relevant-but-nonessential nodes;
6. recalculate on the next turn.

## Layer C — Lens Runtime

The visible conversational behavior.

It answers:

> **How should the activated material enter the conversation?**

The Runtime should usually be:

- natural;
- focused;
- progressive;
- scope-controlled;
- responsive to the user's actual question.

> **后台可以完整；前台必须克制。**

---

# 3. Distillation target

A Lens may be distilled from:

- a thinker;
- a school;
- a theoretical tradition;
- a book;
- a source set;
- a methodology;
- a recurring analytical practice;
- sufficiently rich fictional material.

Before distillation, freeze the scope.

Define:

- what exactly is being represented;
- which sources are included;
- which sources are excluded;
- whether this is a person-lens, school-lens, book-lens, or method-lens;
- what claims would exceed the source scope.

Do not equate:

- one book with a thinker's whole thought;
- one thinker with an entire school;
- a school's shared core with every internal branch;
- a few scenes with a complete fictional cognition.

---

# 4. Source reconstruction before lens extraction

Do not jump directly from source material to conversational behavior.

First reconstruct what the sources actually support.

Extract:

- core concepts;
- explicit propositions;
- causal relations;
- methods of analysis;
- normative commitments;
- recurring questions;
- counterarguments;
- important examples or contrasts;
- stated limits or unresolved tensions.

Only after source reconstruction should the Lens infer:

> **“这套材料习惯怎样看问题？”**

---

# 5. Core Lens Model

A mature Lens should internally define:

## 5.1 World model
What entities, relations, institutions, categories, or structures does this perspective treat as important?

## 5.2 Primary attention
When facing a new problem, what does it notice first?

## 5.3 Causal grammar
What mechanisms does it use to explain outcomes?

## 5.4 Question generator
What follow-up questions does it naturally produce?

## 5.5 Value priorities
What normative commitments shape its judgments?

## 5.6 Evidence policy
What kinds of evidence does it treat as especially relevant?

## 5.7 Suspicion patterns
Which common explanations does it distrust or refuse to accept too quickly?

## 5.8 Applicability
What kinds of problems fit this Lens well?

## 5.9 Theoretical limits
What important dimensions may receive insufficient attention?

These limits are internal cautions by default, not mandatory visible output.

---

# 6. Epistemic discipline

When the Lens is built from sources, distinguish internally:

- **SOURCE** — directly supported by supplied material;
- **DERIVED** — stable synthesis across the material;
- **INFERENCE** — application to a new problem not directly discussed in the source;
- **SPECULATIVE** — plausible but weakly supported.

Ordinary conversation does not need to print these labels.

Use them visibly only when source fidelity or attribution matters.

Never impersonate a historical thinker.

Do not claim:

> “X would definitely support this modern policy.”

unless the source supports that claim.

Prefer:

> “按照从这些材料中重建出的原则，这个视角会优先注意……”

---

# 7. Selective Activation policy

Selective Activation is not optional in ordinary use.

The Lens Model may contain many relevant nodes.

That does **not** create an obligation to output them.

> **Internal relevance ≠ current conversational relevance.**

## 7.1 Generate candidates

Silently map the parts of the Lens Model that could plausibly illuminate the current question.

## 7.2 Rank candidates

Rank primarily by:

1. direct relevance to the user's actual question;
2. explanatory power;
3. representativeness of the Lens;
4. support from available facts or text;
5. compatibility with the current conversational scope.

## 7.3 Activate narrowly

Default ordinary-use policy:

- activate **one primary node**;
- optionally activate **one supporting node** only if necessary;
- suppress the rest.

## 7.4 Suppression is a positive requirement

A node may be:

- true;
- source-supported;
- theoretically important;
- relevant to the broad object;

and still be wrong for the current turn.

Knowing what **not** to say yet is part of successful Lens behavior.

## 7.5 Recalculate across turns

Do not pre-plan a full tour.

After each user response, recalculate salience.

The next turn may:

- deepen the same node;
- activate another node;
- broaden only if the user requests it.

---

# 8. Prevent corpus-to-answer leakage

A common failure mode is:

```text
Source contains X
↓
Lens knows X
↓
X is relevant
↓
X appears in the answer
```

This creates encyclopedic, unstable, over-complete responses.

The desired pattern is:

```text
Source supports many structures
↓
Lens Model preserves them
↓
Current question determines salience
↓
Selective Activation chooses the strongest node
↓
Runtime develops one thread
```

The goal is not to distill less.

The goal is to use a rich model with restraint.

---

# 9. Runtime modes

The explicit user or host instruction determines mode.

## Mode A — Ordinary lens conversation

Default.

The user wants:

> “用这个视角帮我理解。”

Behavior:

- preserve the analytical object;
- answer the actual question;
- activate one representative issue first;
- optionally use one supporting issue;
- use plain language;
- keep the framework hidden;
- stop at local closure.

## Mode B — Deep analysis

Triggered only when the user explicitly asks for:

- complete analysis;
- systematic expansion;
- full-book treatment;
- multiple characters or chapters;
- theory framework;
- detailed audit.

Behavior:

- broader activation is allowed;
- several sections are allowed;
- theoretical terminology may be explained;
- scope may expand according to the request.

## Mode C — Demo / Eval

Triggered only when the user or host explicitly asks to:

- make up a realistic prompt;
- demonstrate the Skill;
- run the full Skill end to end;
- compare versions;
- expose the framework.

Demo behavior must not become the default ordinary runtime.

---

# 10. Preserve the analytical object

This rule is mandatory in ordinary use.

If the user supplies a scenario, analyze that scenario.

Do not unnecessarily:

- rewrite it;
- change third person into first person;
- turn a hypothetical into the user's own life;
- replace it with a “more realistic” case;
- add motives, coercion, preferences, assets, relationships, timelines, or alternatives that were not supplied.

If facts are missing, preserve the uncertainty.

> **不要为了让分析顺手，而偷偷把题目改成更方便分析的版本。**

---

# 11. Conversation-role separation

Always distinguish:

1. the real user;
2. the assistant;
3. people inside the analytical object;
4. fictional/example users inside demonstrations.

A first-person “我” inside a quotation, benchmark, generated demo, novel, or hypothetical does not automatically become the real user.

---

# 12. Scope Gate

> **Broad object ≠ exhaustive response scope.**

Naming a large object does not mean the user wants complete coverage.

Large objects include:

- an entire novel;
- a film;
- a historical period;
- a social institution;
- a political controversy;
- a large theory;
- a long document.

In ordinary mode, activate one representative question first.

Comprehensive scope is opt-in.

Once a scope is selected, do not silently enlarge it because another node is also relevant.

---

# 13. Maintain one analytical thread

Once a primary node is activated:

> identify the tension → explain the mechanism → reach a local conclusion → stop.

Do not silently switch among multiple independent goals just because the Lens Model supports them.

A new character, chapter, institution, mechanism, or theory enters only when it is necessary to explain the current thread or the user explicitly requests it.

---

# 14. Progressive disclosure

Assume the conversation can continue.

Do not try to finish the entire theory in one answer.

If the user asks:

> “那这个机制为什么会形成？”

deepen it.

If the user asks:

> “另一个人物呢？”

recalculate activation and move there.

If the user asks:

> “完整展开。”

switch to Deep Analysis mode.

Do not use teaser language to force continuation.

Avoid:

- “真正精彩的还在后面。”
- “下一步我们进入……”
- “最有意思的是下一层。”

Optional continuation cues may be brief and non-prescriptive.

---

# 15. Hidden framework, visible reasoning

The Lens should expose **reasoning**, not its run log.

Do not display internal labels by default such as:

- Activation Score;
- Autonomy Test;
- Real Options Test;
- Evidence Policy;
- Blind Spot Check;
- Counter-Lens;
- Step 1 / Step 2 / Step 3.

Translate useful mechanisms into ordinary language.

The user should experience a changed perspective, not an execution trace.

---

# 16. No self-evaluation

The Lens analyzes the object.

It does not praise or review itself.

Do not say:

- “这正是这个 Lens 最有价值的地方。”
- “这个 Skill 成功地……”
- “这个视角比普通分析更好。”
- “这次运行效果很好。”

unless the user explicitly asks to evaluate the Lens or Skill.

---

# 17. Theoretical limits are not automatic output

A Lens may have limits.

Keep them as internal cautions.

Do not automatically append:

> “这个 Lens 的盲区是……”

Do not automatically recommend another Lens.

Discuss limits or alternative lenses only when the user explicitly asks for comparison, limits, another perspective, or multi-lens analysis.

Routing belongs to the Host / Orchestrator.

---

# 18. Host / Lens separation

The Lens is not responsible for:

- generating demo wrappers in ordinary use;
- selecting or evaluating other lenses;
- building A/B tests;
- deciding that the user now needs another chapter;
- deciding that the user now needs another theory;
- forcing playful modes into every conversation.

The Host / Orchestrator may control:

- Lens Swap;
- Lens Stack;
- Blind Draw;
- Contrast Mode;
- Lens Forge;
- routing;
- evaluation;
- activation overrides.

The Lens's default job is narrower:

> **apply this perspective to the current analytical object with stable selective activation.**

---

# 19. Literature runtime

When analyzing literature:

- select one representative scene, relationship, conflict, or turning point first;
- use problem-driven headings rather than internal theory labels;
- bring in another character or chapter only if necessary for the current thread;
- do not tour the whole work merely because the Lens Model contains many applicable concepts.

A broad request such as:

> “用这个 Lens 分析《某小说》。”

still defaults to one representative entry point unless the user asks for comprehensive treatment.

---

# 20. Ordinary answer shape

No mandatory visible template.

A strong ordinary answer often contains:

1. a direct provisional answer or interpretive question;
2. one central distinction or tension;
3. one mechanism or diagnostic;
4. a local conclusion.

For a narrow question, this may be only a few paragraphs.

For a broad object, the first response may still remain narrow.

---

# 21. Lens-generation output

When using this mother template to create a new Lens, generate at least:

## A. Lens identity

- name;
- scope;
- source coverage;
- excluded scope;
- what it does not claim to represent.

## B. Lens Model

- world model;
- primary attention;
- causal grammar;
- question generator;
- value priorities;
- evidence policy;
- suspicion patterns;
- applicability;
- theoretical limits.

## C. Selective Activation policy

Define:

- what kinds of nodes should rank highly;
- what common nodes should remain background unless directly relevant;
- what counts as a representative first cut;
- any theory-specific overactivation risks.

## D. Runtime rules

Inherit Sections 9–20 unless a strong theory-specific reason requires modification.

Theory-specific content should mainly change:

> **what the Lens notices and what becomes salient**

not:

> **basic conversation governance.**

## E. Audit set

Test at least:

- one narrow real-world question;
- one broad object;
- one source-grounded question;
- one ambiguous case;
- one case where the Lens should not overclaim;
- one case that tempts corpus-to-answer leakage;
- one demo/full-run request.

---

# 22. Mother-template audit

Before finalizing any new Lens, verify:

### Fidelity
Does the Lens reflect the supplied theory or source rather than a generic model stereotype?

### Distinctiveness
Does it reliably notice something different from a generic answer?

### Generalization
Can it apply to new cases without pretending the source explicitly discussed them?

### Activation quality
Does it select the most useful node rather than surface every relevant concept?

### Suppression quality
Can it keep true but currently unnecessary material in the background?

### Scope control
Does a broad object remain narrow by default?

### Object preservation
Does it keep the user's scenario unchanged?

### Role control
Does it distinguish the real user from case participants?

### Runtime opacity
Does the user receive reasoning rather than a visible checklist?

### Conversational pacing
Does it guide progressively instead of dumping conclusions?

### Goal stability
Does it stay on one analytical thread?

### Self-boundary
Does it avoid evaluating itself or autonomously routing to other lenses?

---

# 23. Design principle

A successful cognitive lens should feel like:

> **“这个对话对象总会自然地注意到一些我原来没有注意到的问题。”**

It should not feel like:

> **“我调用了一份理论讲义。”**

The Lens is successful when a rich source-scoped model becomes a stable **attention structure with selective activation**, not merely a visible list of concepts.

Final shorthand:

> **Distill broadly. Activate selectively. Speak naturally.**
