# GamUX — System Architecture

## Current foundation

The initial GamUX base consists of:

1. Linux kernel.
2. Custom init system.
3. BusyBox.
4. Bash.

The exact versions, configurations, source locations and dependencies have not yet been audited. They must be recorded before modifying or replacing these components.

## Planned layers

### 1. Boot layer

Responsible for starting the operating system.

Components:
- Bootloader.
- Linux kernel.
- Custom init system.

### 2. Base userspace

Responsible for providing essential command-line functionality.

Components:
- BusyBox.
- Bash.
- C library (to be identified).
- Additional system utilities (to be evaluated).

### 3. System services

Responsible for core operating system functionality.

Planned areas:
- Users and permissions.
- Networking.
- Storage.
- Audio.
- Device management.
- Background services.
- Package management.

### 4. Graphics

Responsible for graphical output and hardware acceleration.

Planned areas:
- DRM/KMS.
- Graphics drivers.
- Mesa.
- OpenGL.
- Vulkan.
- Graphical server and window manager.

### 5. Gaming

Responsible for game compatibility and management.

Planned areas:
- Steam.
- Steam Runtime.
- Proton.
- Wine.
- DXVK.
- VKD3D-Proton.
- Third-party Steam-related tools.

### 6. GamUX tools

Utilities developed specifically for GamUX.

Potential tools:
- GamUX CLI.
- Hardware detection.
- Diagnostics.
- Performance profiles.
- Game launcher.

## Architecture principles

- Preserve the existing working base until it has been audited.
- Keep optional gaming components separate from the minimal system.
- Document dependencies and compatibility requirements.
- Keep third-party software distinguishable from GamUX-developed code.
- Test major changes in QEMU before physical deployment.
- Avoid claiming compatibility without testing it.
