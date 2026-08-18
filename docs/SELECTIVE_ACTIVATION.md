# Selective Activation

**Selective Activation** is the layer between a rich Lens Model and the visible conversational Runtime.

Its core principle is:

> **Distill broadly. Activate selectively.**

Chinese shorthand:

> **充分蒸馏，选择性激活。**

---

## Why this layer exists

Source-grounded lens systems often fail in a predictable way:

```text
The source contains many ideas
↓
The internal model knows many ideas
↓
Many of them are technically relevant
↓
The answer tries to include all of them
```

The result is often accurate but conversationally poor:

- theory dumps;
- character or chapter touring;
- constant goal switching;
- unnecessary conclusions;
- long answers that reveal the internal framework;
- responses that feel like reports rather than a perspective.

Cognitive Lenses calls this tendency **corpus-to-answer leakage**.

The solution is not to distill less.

The solution is to insert an explicit activation policy between knowledge and output.

---

## The activation question

The Lens Model asks:

> **What can this perspective notice?**

Selective Activation asks:

> **What deserves to become salient in this turn?**

Runtime asks:

> **How should that activated material enter the conversation?**

These are three different engineering problems.

---

## Default activation policy

For ordinary conversation:

1. preserve the user's exact analytical object;
2. generate candidate cognitive nodes from the Lens Model;
3. rank candidates by current salience;
4. activate one primary node;
5. activate at most one supporting node when necessary;
6. suppress other relevant-but-nonessential nodes;
7. keep one analytical thread;
8. stop at local closure;
9. recalculate activation on the next user turn.

This policy may be relaxed in explicit deep-analysis or demo modes.

---

## Salience criteria

Candidate nodes should be ranked primarily by:

### 1. Direct relevance
Does this node answer the user's actual question?

### 2. Explanatory power
Does it materially change the interpretation, rather than merely add another related fact?

### 3. Lens distinctiveness
Does it reveal something characteristic of this Lens rather than a generic answer?

### 4. Source support
Is the node supported by the source scope or by a clearly marked inference?

### 5. Scope compatibility
Can this node be developed without silently changing the current analytical goal?

---

## Suppression is part of intelligence

Selective Activation is not only about choosing what to say.

It also requires knowing what **not** to say yet.

A node may be:

- true;
- source-supported;
- theoretically important;
- relevant to the broad object;

and still be wrong for the current turn.

Therefore:

> **Internal relevance ≠ current conversational relevance.**

A stable Lens must be able to keep useful knowledge in the background.

---

## Broad object does not change the rule

A broad analytical object does not justify activating more nodes by default.

If the user names:

- an entire novel;
- a theory;
- a social institution;
- a historical period;
- a large source set;

the ordinary activation policy still prefers one representative issue first.

> **Broad object ≠ exhaustive answer.**

Comprehensive activation is opt-in.

---

## Recalculation across turns

Selective Activation is dynamic.

Turn 1 may activate node A.

The user's response may make node B newly salient.

The Lens should then recompute rather than continue a prewritten tour.

```text
Turn 1 question
↓
Activate A
↓
Local closure
↓
User response
↓
Re-rank candidates
↓
Activate B or deepen A
```

This is why Cognitive Lenses treats conversation as multi-turn by default.

---

## Activation vs summarization

Summarization asks:

> What information should be compressed and retained?

Selective Activation asks:

> Of everything already retained, what should become active now?

The two can coexist.

A Lens may be built from a highly compressed source model and still require selective activation at runtime.

---

## Activation vs persona behavior

Persona systems often try to maintain:

- voice;
- temperament;
- behavioral consistency;
- role identity.

Selective Activation instead controls:

- salience;
- problem framing;
- question priority;
- explanatory focus;
- suppression of nonessential cognitive nodes.

It is therefore closer to an **attention policy** than a personality script.

---

## Host interaction

The Host / Orchestrator may modify activation policy intentionally.

Examples of host-level changes include:

- deep-analysis mode;
- contrast mode;
- lens stacking;
- explicit multi-node expansion;
- evaluation mode.

But a single Lens should remain usable without a complex Host.

Its default activation behavior should be stable on its own.

---

## Audit questions

A Lens fails Selective Activation when:

- it surfaces every relevant concept;
- it changes goals repeatedly in one answer;
- it tours many chapters or characters without request;
- it treats a broad object as permission for exhaustive analysis;
- it exposes its internal checklist;
- it keeps adding conclusions after the current issue is already resolved.

A Lens passes when:

- one representative mechanism becomes clear;
- related but unnecessary material stays silent;
- the answer reaches local closure;
- the next turn can legitimately activate a different part of the Lens Model.

---

## Short form

```text
Distill broadly
↓
Preserve a rich Lens Model
↓
Rank by current salience
↓
Activate selectively
↓
Speak naturally
↓
Stop locally
↓
Recompute on the next turn
```

That is the intended runtime behavior of Cognitive Lenses.
