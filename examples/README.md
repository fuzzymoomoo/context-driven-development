# Examples

These examples are intentionally small and platform-neutral. They are here to make the method easier to reason about, not to prescribe one implementation stack.

## 1. Same prompt, different context

Prompt:

`Design a customer onboarding workflow`

### Weak context

- only the prompt

Likely result:

- generic flow
- missing domain constraints
- inconsistent naming
- no validation expectations

### Strong context

- business goal
- user roles
- compliance constraints
- data ownership rules
- existing service boundaries
- prior validated workflow example

Likely result:

- bounded design
- fewer invalid assumptions
- clearer integration points
- better validation targets

The prompt stayed simple. The context changed. The outcome changed.

## 2. Minimal stage flow

1. identify the current context delta
2. assemble the bounded context bundle
3. decide whether the context is sufficient
4. execute the stage
5. validate the output
6. promote only validated outputs into future context

## 3. Probabilistic and deterministic side by side

### Probabilistic stage

Task:

`Propose a service boundary for invoice dispute handling`

Why it is probabilistic:

- interpretation is required
- tradeoffs are involved
- more than one acceptable design may exist

### Deterministic stage

Task:

`Generate the service scaffold from the approved contract`

Why it is deterministic:

- the structure is already decided
- the output shape is constrained
- repeatability matters more than interpretation

## 4. Context bundle to validated output

Initial need:

`Add a retention-policy review feature`

Context bundle:

- policy requirements
- user roles
- system constraints
- domain terms
- existing review workflow patterns
- output contract for the feature proposal

Execution output:

- feature proposal
- workflow sketch
- validation checklist

Validation:

- does it fit the domain language?
- does it respect policy constraints?
- is the output complete enough for the next stage?

Only after validation should the result influence later work.
