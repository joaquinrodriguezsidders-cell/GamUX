# GamUX

**A lightweight Linux distribution focused on gaming and low-resource hardware.**

GamUX is an experimental Linux distribution designed to provide a lightweight, modular gaming operating system, with a particular focus on older computers and resource-constrained hardware.

## Project status

**Early development — experimental. Not ready for daily use.**

## Initial system foundation

GamUX starts from an existing Linux system composed of:

- Linux kernel
- Custom init system
- BusyBox
- Bash

The existing components will be preserved while their source code, configuration, dependencies and boot process are progressively audited and documented.

## Main goals

- Minimize idle RAM and CPU consumption.
- Support older hardware where technically possible.
- Provide Linux gaming compatibility.
- Support Steam and relevant gaming technologies.
- Keep optional components separate from the minimal base.
- Make builds reproducible and maintainable.

## Repository structure

- `boot/` — Bootloader, kernel and init.
- `base/` — Essential userspace components.
- `system/` — Networking, users, storage, audio and services.
- `graphics/` — Graphics drivers and rendering stack.
- `gaming/` — Steam, Proton and gaming integrations.
- `tools/` — GamUX-specific utilities.
- `build/` — Build scripts, packages and toolchain.
- `config/` — Default system configurations.
- `tests/` — System and performance tests.
- `iso/` — Bootable image construction.
- `docs/` — Project documentation.

## Development strategy

Development starts in QEMU virtual machines. Physical hardware testing will be introduced progressively, initially using a Dell OptiPlex 360.

## Documentation

- [Project vision](docs/VISION.md)
- [Roadmap](docs/ROADMAP.md)
- [Architecture](docs/ARCHITECTURE.md)
- [Building](docs/BUILDING.md)
- [Testing](docs/TESTING.md)
- [Hardware](docs/HARDWARE.md)

## Third-party software

GamUX may integrate third-party projects. Their source code, licenses, trademarks and distribution requirements remain separate and must be respected.

GamUX is independent and is not affiliated with Valve or the developers of third-party projects.

## Contributions

See [CONTRIBUTING.md](CONTRIBUTING.md).
