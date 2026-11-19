# Building GamUX

## Status

The build process has not yet been finalized.

GamUX currently starts from an existing Linux base. The first task is to identify how that base was built and reproduce its current state before changing it.

## Development host

The initial development host is Windows.

QEMU will be used to test bootable system images. Linux-based build tooling may be introduced as the build process requires it.

## Build requirements to determine

- Kernel source and version.
- Kernel configuration.
- Custom init source and build instructions.
- BusyBox source, version and configuration.
- Bash source, version and configuration.
- C library and compiler toolchain.
- Root filesystem layout.
- Bootloader and image-generation procedure.

## Build principles

1. Record exact source versions.
2. Keep configuration files under version control.
3. Do not commit generated binaries or large build artifacts.
4. Document dependencies.
5. Keep build logs for troubleshooting.
6. Prefer reproducible build procedures.
7. Test each generated image in QEMU.

## First milestone

Reproduce the existing minimal system and boot it in QEMU without changing its behavior.
