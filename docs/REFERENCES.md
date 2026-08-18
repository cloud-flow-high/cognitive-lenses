# References & Design Basis

Cognitive Lenses is an experimental workflow. The references below are **design inspirations and adjacent foundations**, not evidence that this exact architecture is an established academic standard.

## AI Skill format

### OpenAI — Using skills
OpenAI describes Skills as reusable workflows, generally centered on a portable `SKILL.md` playbook with instructions and supporting resources.

https://openai.com/academy/skills/

### OpenAI Help Center — Skills in ChatGPT
Documents creation, upload, sharing, installation, and the portable Skills workflow in ChatGPT.

https://help.openai.com/en/articles/20001066

## Framing as a reasoning concept

### Nguyen, Chari & Sayre — Dynamics of students' epistemological framing in group problem solving
Discusses epistemological framing as a way people decide what knowledge is relevant and how to proceed in a problem.

https://arxiv.org/abs/1607.03019

### Tuveri, Steri & Fanti — Problem Framing in the AI era: a new model
Explores problem framing in AI-assisted reasoning contexts.

https://arxiv.org/abs/2503.17040

### Apartsin & Aperstein — Framing, Judging, Steering
Proposes separating framing, judging, and steering in human-AI co-reasoning.

https://arxiv.org/abs/2606.05983

## Project-specific synthesis

The following ideas are **project-level engineering conventions developed through prototype iteration**, rather than claims taken directly from the references above:

- source-scoped Lens identity;
- Source Reconstruction before Lens extraction;
- Lens Model / Selective Activation / Runtime separation;
- Selective Activation as an explicit relevance policy;
- `Distill broadly. Activate selectively.`;
- corpus-to-answer leakage as a runtime failure mode;
- Scope Gate;
- Broad object ≠ exhaustive answer;
- Internal relevance ≠ current conversational relevance;
- one-primary-node default activation;
- suppression of relevant-but-nonessential nodes;
- progressive disclosure and per-turn reactivation;
- Host / Lens responsibility separation;
- no self-evaluation;
- no automatic cross-lens routing;
- forkable cognitive-perspective packages.

These conventions should be evaluated as engineering choices: by stability, source fidelity, distinctiveness, generalization, activation quality, scope control, and conversational usefulness.
