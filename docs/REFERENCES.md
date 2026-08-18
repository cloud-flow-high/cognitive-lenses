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

The following ideas are project design decisions developed through prototype iteration rather than claims taken directly from the references above:

- Lens Model / Lens Runtime separation;
- Scope Gate;
- Representative-topic selection;
- Progressive disclosure;
- Internal relevance ≠ current conversational relevance;
- Host / Lens responsibility separation;
- no self-evaluation;
- no automatic cross-lens routing;
- source-scoped lens identity;
- forkable cognitive-perspective packages.

These should be treated as engineering conventions of this project.
