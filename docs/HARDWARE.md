# GamUX — Hardware Support

## Initial test platforms

### QEMU

The initial virtual test platform.

It will be used for:
- Boot testing.
- Init testing.
- Root filesystem testing.
- Repeatable memory-limit experiments.
- Regression testing.

### Dell OptiPlex 360

An initial physical test machine.

Exact specifications are not yet documented.

Before hardware compatibility testing, record:
- CPU model.
- Installed RAM.
- GPU model.
- Storage type and capacity.
- Network adapter.
- Audio device.
- BIOS version and boot capabilities.

## Compatibility policy

GamUX aims to support older hardware where practical.

Hardware support must be based on actual testing. Virtual machine results do not prove that a physical GPU, audio device or network adapter works.
