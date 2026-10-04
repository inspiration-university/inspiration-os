# Modeling Guidelines

MindScript makes causal models easy to write. That also makes it easy to write overconfident models.

Use the following conventions to preserve intellectual humility.

## Observation vs interpretation

Prefer:

```mind
OBSERVED:
    contactBecomesIntermittent

ASSUMES:
    validationSeeking
        confidence = medium
```

rather than treating inferred motive as observed fact.

## State vs identity

Prefer:

```mind
WHEN:
    criticismDetected

DO:
    defensiveResponse()
```

rather than:

```text
"Person is defensive."
```

## Hypotheses

Many Inspiration OS scripts are working models rather than established scientific constructs.

Use MindScriptDoc status labels such as:

```text
@status established
@status supported
@status hypothesis
@status metaphor
@status experimental
```

## Naming

Memorable names are useful, but names do not turn a model into a diagnosis.

Examples such as `rescuedPuppySyndrome()` or `princessInHighCastle()` should be treated as descriptive metaphors.

## Useful failure

A good model should expose where it can fail.

Use `RISKS` for:
- false positives
- overgeneralization
- maladaptive escalation
- unintended social effects
- conditions under which the model stops being useful
