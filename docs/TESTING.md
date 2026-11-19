# GamUX — Testing Strategy

## General rule

Every major system change must be tested before being considered complete.

## Virtual machine testing

QEMU is the initial testing environment.

Tests should cover:
- Kernel startup.
- Init execution.
- Root filesystem mounting.
- Essential device filesystems.
- BusyBox commands.
- Bash startup.
- Console operation.
- Shutdown and reboot.

## Physical hardware testing

The Dell OptiPlex 360 is an initial hardware test target.

Its exact CPU, RAM, GPU, storage and firmware configuration must be recorded before drawing compatibility conclusions.

## Performance testing

Record:
- Total RAM.
- Available RAM.
- Process memory usage.
- CPU usage while idle.
- Boot time.
- Storage usage.
- Driver and device information.

Compare measurements only when the test conditions are equivalent.

## Reporting failures

A useful bug report includes:
- Hardware or VM configuration.
- GamUX revision.
- Steps to reproduce.
- Expected behavior.
- Actual behavior.
- Relevant logs.
