# Inspiration OS Architecture

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

## MindScript

The language used to express processes and causal models:

https://github.com/inspiration-university/mind-script

## Prometheus Kernel

Minimal reusable primitives.

## Standard Library

Higher-level behavioral, emotional, social, and organizational scripts.

## Apps

Intentional practices that inspect, modify, reinforce, or replace scripts.

## Distros

Curated combinations of scripts, practices, values, and defaults for different modes of living or working.

## Design principle

Lower layers should not depend on higher layers.

The kernel should know nothing about MuseOS or FoundryOS. Distros may depend on everything below them.
