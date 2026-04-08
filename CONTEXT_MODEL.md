# CDD Context Model

## Purpose

The CDD Context Model defines the operating shape behind the methodology.

It extends the basic CDD loop into a broader model where:

- contexts hold governed truth and decision pressure
- plans formalize responses to context
- tasks execute plans
- outputs update context only after validation
- views render useful projections for different audiences

The point is to organize work around context, validated response, and feedback rather than around disconnected boards or task lists.

## Core doctrine

### There are only contexts, plans, and outputs

Everything else is a view.

Backlogs, dashboards, roadmaps, and boards can all be useful, but they are projections over the real control surfaces rather than the source of truth.

### Context is the control surface

Context is not passive background information. It shapes what should happen next.

### Context creates decision pressure

Contexts do not just store facts. They create pressure on decisions.

Examples:

- strategic context pressures priority
- operational context pressures stability and readiness
- execution context pressures bounded delivery
- reflective context pressures learning and improvement

### Plans are responses to context

A plan is a validated semantic response to one or more contexts.

### Tasks are emitted, not primary

Tasks are operational units produced by plans. They are important, but they are not the top-level organizing concept.

### Outputs must be validated before they update context

Execution does not automatically become future truth.

### History and feedback are first-class

Significant decisions and changes should be traceable over time.

### Generalization is governed

Repeated success can become reusable capability, but only through explicit review and validation.

## Operating loop

The broader CDD loop is:

`Context Delta -> Plan Selection -> Context Assembly -> Plan Validation -> Task Emission -> Execution -> Output Validation -> Context Update -> History / Generalization`

### Context delta

Something meaningful changes:

- a business priority shifts
- a system health signal appears
- a release readiness gate fails
- a reusable pattern emerges

### Plan selection

The system determines whether a plan is needed and what type of plan best fits the situation.

### Context assembly

The relevant context is assembled into a bounded bundle for the current stage.

### Plan validation

The proposed response is checked for validity and sufficiency.

### Task emission

Executable units are emitted into the delivery surfaces a team uses, such as issue trackers, branches, reviews, or deployment workflows.

### Execution

Work is performed by people, AI systems, deterministic generators, or hybrids.

### Output validation

Outputs are checked before they become future truth.

### Context update

Validated outputs update the relevant contexts.

### History and generalization

The event is recorded, and repeated success may be generalized into stronger future capability.

## Universal context contract

Every context type should share a common shape even when the meaning differs.

At a conceptual level, a context should define:

```yaml
context:
  id: string
  contextType: string
  title: string
  purpose: string
  owner: string
  status: draft | active | inactive | archived

  description:
    summary: string
    detail: string

  sources: []
  links: []
  signals:
    observations: []
    risks: []
    opportunities: []
    pressures: []

  state:
    currentState: string
    confidence: low | medium | high
    freshness: string
    validationStatus: valid | provisional | stale | invalid

  governance:
    visibility: public | internal | restricted
    updateRules: []
    validationRules: []

  provenance:
    assembledBy: string
    assembledAt: datetime
    updatedBy: string
    updatedAt: datetime
    activeInputs: []
```

The exact schema can vary by implementation, but the model requires the same underlying concepts:

- where the context came from
- what it is linked to
- what it is currently saying
- how trustworthy and current it is
- what governance applies
- how it was assembled and changed

## Context families

CDD groups contexts into four major families.

### Strategic contexts

Explain why work should exist.

- business context
- vision context

### Operational contexts

Explain what is happening in reality now.

- system context
- deployment context
- release context

### Execution contexts

Explain what is actively being worked on and under what bounds.

- development context
- knowledge context

### Reflective contexts

Explain how the system learns, remembers, and improves.

- history context
- prediction context
- generalization context

## Plans, tasks, outputs, and views

### Plans

Plans interpret context and define a bounded response.

They should link to:

- at least one driving context
- any supporting contexts
- the planning mode used
- the intended next stages

Plans are semantic: they capture meaning, scope, rationale, and direction.

### Tasks

Tasks are executable units emitted from validated plans.

They should never float without meaning. Every task should trace back to:

- a plan
- a context bundle
- a success path

Tasks are operational.

### Outputs

Outputs are the results of execution.

Examples:

- specifications
- code
- tests
- deployments
- releases
- documents
- decisions
- templates
- validators

Outputs influence future work only after validation.

### Views

Views are projections for a particular audience or purpose.

Examples:

- executive priority view
- system health view
- developer work view
- release readiness view
- knowledge lineage view
- history timeline view

Views are useful, but they are not the truth.

## Context mesh

CDD does not treat contexts as a flat list or a simple sequence. Contexts form a mesh.

Examples:

- strategic context influences execution context
- operational context escalates into strategic concern
- history informs prediction
- generalization improves future knowledge and execution

The doctrine is simple:

- CDD operates over a context mesh
- plans move through the mesh
- views render slices of it

## Relationship rules

The model depends on a few strict rules:

1. Every plan must link to context.
2. Every task must link to a plan.
3. Every output must be validated before updating context.
4. Every important change should leave history.
5. Generalization requires governance.
6. Prediction is advisory only.

## Practical doctrine statements

- There are only contexts, plans, and outputs. Everything else is a view.
- The board is not the truth. The board is a projection.
- Context determines what should happen next.
- Plans interpret. Tasks execute. Outputs update.
- Generalization governs what becomes reusable truth.
