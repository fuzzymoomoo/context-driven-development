# FAQ

## Is this just prompt engineering?

No.

CDD treats prompting as one possible execution surface inside a larger governed system. The key question is not "what prompt did we write?" but "what context was assembled, what output was expected, and what validation happened afterward?"

## How is this different from spec-driven development?

Spec-driven development is one important ingredient, but CDD is broader.

CDD includes:

- knowledge and decision context
- stage-aware context assembly
- validation before truth is updated
- provenance
- feedback and generalization

Specifications can be part of the context bundle, but they are not the entire system.

## Does this require AI?

No.

CDD applies to human work, deterministic generators, AI-assisted workflows, and combinations of all three. AI makes the need for better context more visible, but the method is not AI-only.

## Is this a process framework or a tool?

It is a methodology first.

Tools can help express it, but the method is not tied to one product, editor, or stack.

## Where do deterministic generators fit?

CDD treats deterministic generators as execution systems that materialize already-governed context. They are the natural fit where outputs should be strict and repeatable.

## Is CDD anti-human?

No.

CDD is designed to improve collaboration between humans and machines by making the governing context more explicit, portable, and reviewable.

## Is CDD a replacement for planning and review?

No.

CDD makes planning and review more structured. It does not remove the need for judgment, validation, or governance.

## How is a wave different from a sprint or a stage?

A **wave** is a bounded, cross-cutting delivery slice chosen from a broader plan for current execution.

It is not the same as:

- a **sprint**, which is usually a time box
- a **stage**, which is a defined execution mode in the CDD model
- a **task**, which is an emitted operational unit

Teams often need a practical unit for "the coordinated body of change we are doing now." In CDD, that is the wave.

## Why is this first public release docs-only?

Because the methodology needs to be clear before any public reference tooling can be responsibly shaped around it.
