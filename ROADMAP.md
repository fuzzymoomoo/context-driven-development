# Public Roadmap

## Current release

This repository is the first public, docs-first release of CDD.

The current goal is to make the core ideas stable, understandable, and discussable in public before publishing reference implementations or tooling.

## Track 1: Methodology and docs

Near-term work:

- refine the public manifesto
- stabilize the context model
- expand the glossary and FAQ
- publish more worked examples
- clarify planning modes, context sufficiency, and output contracts

Success looks like:

- a cold reader can understand the core method quickly
- the terminology stays consistent
- the public docs can stand on their own without a tool dependency

## Track 2: Reference examples

Future public work:

- small, public-safe examples of context bundles
- example stage flows
- minimal planning-mode examples
- examples showing probabilistic and deterministic execution side by side

Success looks like:

- contributors can see how the method applies in practice
- examples remain platform-neutral and easy to adapt

## Track 3: Future open tooling

Later public work may include:

- lightweight reference tooling
- context assembly examples
- validation helpers
- open reference implementations of selected parts of the method

This work should follow the docs, not outrun them.

Success looks like:

- tooling expresses the method clearly
- the public tool surface does not overfit one private stack
- the open implementation proves the ideas without pretending to be the final enterprise shape

## Deliberate non-goals for v0

- publishing private implementation planning
- publishing machine-local workflow tooling
- publishing private runtime assumptions
- forcing the method to depend on one editor, one model provider, or one memory layer

## Guiding principle

The public direction should remain clear:

CDD is a method first. Public examples come next. Public tooling follows when it can express the method cleanly.
