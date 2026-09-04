# bonsai/think

**Think is the method layer of the bonsai agent organization.**

`bonsai/intelligence` defines what intelligence is.
`bonsai/think` defines how intelligence thinks.
`bonsai/company` defines who thinks and acts.

## Position

```text
bonsai/intelligence
        ↓
      THINK
        ↓
bonsai/company
        ↓
      Agents
        ↓
     Actions
```

## Definition

> **Think = a reusable method for turning goals, observations, knowledge, evidence, and uncertainty into better decisions.**

A Think method is not an agent and not an LLM prompt. It is a named, inspectable, composable procedure that an agent can select and execute.

## Core loop

```text
Observe
  ↓
Frame
  ↓
Gather Evidence
  ↓
Relate
  ↓
Hypothesize
  ↓
Reason
  ↓
Compare Alternatives
  ↓
Decide
  ↓
Act
  ↓
Evaluate
  ↓
Learn
  └──────────────→ Observe
```

## Method contract

Each method should define:

- `purpose` — what problem it solves
- `inputs` — required observations/knowledge/evidence
- `steps` — reasoning procedure
- `constraints` — what must not be assumed
- `outputs` — decision, hypothesis, plan, or action
- `evidence` — basis for the conclusion
- `uncertainty` — confidence and unknowns
- `feedback` — how results improve future use

## Principles

1. **Method before model** — an LLM may implement a step, but the method is model-independent.
2. **Evidence before assertion** — conclusions should be traceable to evidence.
3. **Alternatives before commitment** — decisions should expose meaningful alternatives.
4. **Uncertainty is data** — unknowns and confidence are first-class.
5. **Feedback closes the loop** — outcomes become learning inputs.
6. **Composable methods** — methods can call or combine other methods.
7. **Agents select methods** — `bonsai/company` supplies organizational context; Think supplies the cognitive procedure.

## Examples

```text
scan
classify
compare
decompose
synthesize
hypothesize
validate
prioritize
forecast
diagnose
plan
review
reflect
```

## Relationship to the bonsai system

```text
Intelligence  = capability
Think         = method
Company       = organization
Agent         = actor
Archimedes    = architect agent
Repos         = memory / observation
BQML          = discovery
Ontology      = meaning
AW            = execution
GitHub        = source of truth
```

Filesystem is storage. Metadata is memory. Search is access. Ontology is meaning. **Think is method. Company is organization.**
