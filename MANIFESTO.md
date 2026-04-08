# CDD Manifesto

## The premise

Software is built by controlling context, not by trusting improvisation.

That is the core belief behind Context-Driven Development.

CDD does not begin with a model, a prompt, or a generator. It begins with the understanding that every meaningful software outcome is shaped by context:

- the problem framing
- the constraints
- the architecture
- the prior knowledge
- the conventions
- the examples
- the validation rules

When these are weak, hidden, or inconsistent, output quality becomes fragile. When they are explicit, structured, and governed, outcomes become more predictable.

## Context is the control surface

Context is not background information. It is the primary control layer.

In CDD, the goal is not to "get a good answer" from a system through clever prompting. The goal is to shape the environment in which work happens so that good answers become more likely and bad answers become easier to detect.

That applies whether the work is done by:

- a human engineer
- an AI assistant
- a code generator
- a hybrid workflow across all three

## Prompting is not the system

Prompting can be useful, but prompting alone is not a reliable operating model.

A prompt without governed context is just an instruction floating without enough structure. CDD argues that quality comes from the surrounding system:

- what context is available
- what stage is being performed
- what output shape is expected
- what validation must happen
- what becomes future truth

Prompting is only one expression surface inside that larger system.

## Two execution modes

CDD recognizes that not all work is the same.

### Probabilistic execution

Some work requires interpretation, synthesis, or design. In those cases, context does not determine the exact result, but it changes the quality and direction of the probability distribution.

This includes work such as:

- planning
- architecture
- design
- synthesis
- exploratory authoring

### Deterministic execution

Other work should be strict and repeatable. In those cases, context defines what should be materialized and the system should not improvise beyond those boundaries.

This includes work such as:

- scaffolding
- template generation
- schema-driven transformation
- repeatable code production

CDD exists to handle both modes coherently.

## Validation is part of the method

CDD does not stop at generation or execution.

Outputs must be validated before they are trusted and before they are allowed to influence later work. Speed without validation simply moves error downstream faster.

Validation may include:

- structural checks
- alignment checks
- completeness checks
- convention checks
- context sufficiency checks

Only validated outputs should become future context.

## Provenance matters

Teams need to know why an output looks the way it does.

That means tracking:

- what context was active
- what constraints were present
- what prior outputs or references were used
- who or what performed the work
- what validation happened

Provenance turns opaque generation into auditable reasoning about the conditions that shaped a result.

## Feedback matters

CDD includes an explicit improvement loop.

When a pattern works repeatedly, it should not remain accidental forever. It can be extracted, reviewed, and generalized into stronger defaults, templates, validators, or stage definitions.

This is how the system gets better over time:

- probabilistic work becomes more guided
- repeatable work becomes more deterministic
- lessons become reusable capability

## What CDD is not

CDD is not:

- a license to let AI loose in a codebase
- a synonym for prompt engineering
- a rejection of engineering discipline
- a claim that all work can be automated
- a replacement for judgment, review, or governance

CDD is a method for moving discipline up into the context layer so execution becomes safer and more coherent.

## The outcome

When CDD is working well:

- the system knows what context a stage needs
- work is easier to route and bound
- outputs are easier to validate
- teams can explain what shaped a result
- successful patterns become reusable rather than repeatedly rediscovered

The point is not just faster generation.

The point is better-governed outcomes.
