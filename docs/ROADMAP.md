# GamUX — Development Roadmap

This roadmap describes the intended development order. Items are not considered complete until they have been tested and documented.

## Phase 0 — Repository and audit

- [x] Create the Git repository.
- [x] Establish the initial directory structure.
- [x] Document the initial project direction.
- [ ] Identify the exact kernel version and configuration.
- [ ] Locate and document the custom init source code.
- [ ] Identify BusyBox version and configuration.
- [ ] Identify Bash version and dependencies.
- [ ] Document how the existing system currently boots.
- [ ] Establish a reproducible development environment.

## Phase 1 — Minimal bootable system

- [ ] Boot the existing system in QEMU.
- [ ] Verify kernel startup.
- [ ] Verify execution of the custom init.
- [ ] Verify procfs, sysfs and devtmpfs mounts.
- [ ] Verify BusyBox utilities.
- [ ] Verify Bash.
- [ ] Verify console input and output.
- [ ] Verify shutdown and reboot.
- [ ] Capture useful boot logs.

## Phase 2 — Base operating system

- [ ] Audit the C library and userspace dependencies.
- [ ] Document essential system utilities.
- [ ] Implement or verify user and permission management.
- [ ] Implement or verify storage support.
- [ ] Implement networking.
- [ ] Evaluate package management.
- [ ] Establish package versioning and update procedures.

## Phase 3 — Graphics and desktop

- [ ] Identify supported graphics hardware.
- [ ] Integrate appropriate kernel graphics drivers.
- [ ] Integrate Mesa where appropriate.
- [ ] Evaluate OpenGL and Vulkan support.
- [ ] Evaluate a lightweight graphical environment.
- [ ] Implement audio support.
- [ ] Test on physical hardware.

## Phase 4 — Gaming

- [ ] Evaluate Steam compatibility.
- [ ] Evaluate Steam Runtime requirements.
- [ ] Integrate Proton and Wine where appropriate.
- [ ] Evaluate DXVK and VKD3D-Proton.
- [ ] Verify 32-bit compatibility.
- [ ] Test games on supported hardware.

## Phase 5 — GamUX tools

- [ ] Evaluate Aurelia.
- [ ] Evaluate SteamFlow.
- [ ] Evaluate SteamKit.
- [ ] Evaluate DepotDownloader.
- [ ] Design the GamUX CLI.
- [ ] Develop game management tools.

## Phase 6 — Optimization

- [ ] Establish a reproducible idle-memory benchmark.
- [ ] Measure CPU and memory usage.
- [ ] Evaluate background services.
- [ ] Evaluate zram and memory-management options.
- [ ] Test older CPUs and GPUs.
- [ ] Compare performance against a documented baseline.

## Phase 7 — Distribution

- [ ] Automate system builds.
- [ ] Generate a bootable ISO.
- [ ] Create an installer.
- [ ] Establish signed updates and rollback mechanisms.
- [ ] Publish an experimental release.
