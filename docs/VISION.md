# GamUX — Project Vision

## Purpose

GamUX aims to create a lightweight Linux distribution focused on gaming, especially on older computers and systems with limited hardware resources.

## Main objectives

1. Keep the base operating system as small as reasonably possible.
2. Minimize unnecessary background services and resource consumption.
3. Preserve compatibility with older CPUs and GPUs whenever technically possible.
4. Support modern Linux gaming technologies where hardware permits.
5. Provide convenient tools to install, manage and launch games.
6. Keep optional functionality separate from the minimal base.

## Design principles

- **Minimalism:** only essential components should run by default.
- **Modularity:** optional features should not unnecessarily increase base resource usage.
- **Compatibility:** hardware support matters more than size alone.
- **Reproducibility:** builds should be repeatable and documented.
- **Security:** updates, packages and credentials must be handled safely.
- **Measurability:** performance claims must be supported by tests.

## Initial performance target

An initial research target is approximately 200 MB of RAM usage at idle.

This is a development goal, not a guaranteed specification. Actual memory usage depends on hardware, drivers, services and the selected graphical environment.

Measurements must distinguish base-system memory use from filesystem cache, buffers and other reclaimable memory.

## Initial foundation

The project starts from an existing Linux kernel, a custom init system, BusyBox and Bash.

These components will be audited before major architectural changes are made.

## Development philosophy

GamUX will be developed incrementally. Each system layer must be tested before additional complexity is introduced.
