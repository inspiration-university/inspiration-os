# Inspiration OS 🔥

*An open framework for inspecting, composing, and evolving human behavioral scripts.*

Inspiration OS treats beliefs, habits, emotional responses, decision rules, and social dynamics as **inspectable and composable processes** rather than fixed traits.

It is written in [MindScript](https://github.com/inspiration-university/mind-script), a human-readable language for modeling behavior and causal systems.

## Architecture

```text
MindScript
    ↓
Prometheus Kernel
    ↓
Standard Library
    ↓
Apps
    ↓
Distros
```

### MindScript

The language. It defines script calls, state, conditions, loops, dependencies, and readable causal logic.

### Prometheus Kernel

The smallest reusable primitives: reality evaluation, value comparison, risk assessment, state updates, learning, and basic emotional processes.

See [kernel/](kernel/).

### Standard Library

Reusable higher-level models such as:

- `missionImpossibleDrive()`
- `cannotBeBothered()`
- `accountabilityResponse()`
- `shield()` / `bridge()`
- `comfortBeacon()`
- `idealizationShield()`
- `rescuedPuppySyndrome()`
- `prestigeBrandElevation()`
- `dictatorshipDilemma()`

See [library/](library/).

### Apps

Intentional practices that inspect, modify, reinforce, or replace scripts.

Current examples include morning rituals, shadow work, and vision mapping.

See [apps/](apps/).

### Distros

Curated combinations of scripts, values, practices, and defaults for different modes of living or working.

Current distro concepts include:

- MuseOS
- FoundryOS
- PhoenixOS
- SeekerOS

See [distros/](distros/).

## A simple example

```mind
bridge(problem) {

    BELIEF:
        "Accepting responsibility gives me power to fix things."

    WHEN:
        responsibilityDetected

    DO:
        acknowledgeMyRole()
        validateImpact()
        confirmUnderstanding()
        offerSolution()
        followThrough()

    RETURN:
        repair
}
```

The point is not to claim that people literally execute code.

The point is to make recurring patterns explicit enough to inspect, question, compare, test, and replace.

## Modeling principles

- Prefer processes over identity labels.
- Separate observation from interpretation.
- Mark speculative models as hypotheses.
- Keep MindScript readable by non-programmers.
- Treat models as tools, not diagnoses.
- Prefer small composable scripts over giant explanations.
- Use scenarios and outcomes to test whether a model is actually useful.

## Repository map

```text
kernel/     Prometheus primitives
library/    reusable MindScript models and conceptual modules
apps/       intentional practices
distros/    curated Inspiration OS distributions
docs/       architecture and modeling documentation
```

## Status

Inspiration OS is experimental and evolving.

The current focus is building a coherent standard library and using real examples to discover which MindScript constructs are genuinely useful.

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md).

## License

GNU GPL v3. See [LICENSE](LICENSE).

---

**Inspiration is not scarce. It is badly distributed.**
