# Contributing to Inspiration OS

We welcome contributions that improve the clarity, usefulness, and composability of Inspiration OS.

## Architecture

Before adding a file, decide which layer it belongs to:

- `kernel/` — minimal reusable primitives
- `library/` — higher-level behavioral or causal scripts
- `apps/` — intentional practices that operate on scripts or state
- `distros/` — curated combinations of lower-level components
- `docs/` — architecture, modeling, and contributor guidance

MindScript itself lives in a separate repository:

https://github.com/inspiration-university/mind-script

## Adding a script

Prefer one focused process per `.mind` file.

Use camelCase:

```mind
evaluateRisk()
missionImpossibleDrive()
offerConfirmReturnAgency()
```

Add comments generously, especially when a construct could otherwise be mistaken for a factual claim about another person's motives.

Where appropriate, document status:

```java
/**
 * @status hypothesis
 */
```

## Modeling guidelines

- Separate `OBSERVED` behavior from `ASSUMES` interpretations.
- Do not present a hypothesis as a diagnosis.
- Prefer "this script may run under these conditions" over "this person is X."
- Include `RISKS` when a useful script can become maladaptive.
- Include `REPLACEMENT` when a safer or more effective alternative is known.
- Keep scripts compact enough to understand at a glance.

## Contributing workflow

1. Fork the repository or create a branch.
2. Add or revise the relevant script/module.
3. Explain the modeling problem and assumptions.
4. Open a pull request.
5. Be willing to revise both the model and the syntax if examples expose weaknesses.

## Distros

A distro should compose existing components rather than duplicate them.

Prefer:

```mind
foundryOS() {

    REQUIRES:
        purpose()
        missionImpossibleDrive()
        bridge()
}
```

over copying the implementation of each dependency into the distro itself.

## Style

Keep it inclusive, non-dogmatic, falsifiable where possible, and accessible to non-programmers.
