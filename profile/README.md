# EdgeOS Project

EdgeOS is an independent operating-system project focused on running familiar
Linux userspace across x86_64 and ARM64 while keeping architecture-neutral
kernel behavior in shared code.

## Repositories

- [kernel](https://github.com/EdgeOS-Project/kernel) contains the EdgeOS
  kernel, shared Linux-compatible ABI implementation, architecture ports,
  drivers, build configuration, and validation tools.
- [workstation](https://github.com/EdgeOS-Project/workstation) contains the
  QEMU-based VM manager, graphical console, lifecycle tools, and desktop test
  workflow.

Distribution images will be published as versioned release artifacts after the
source and reproducibility workflow is ready. Test-only userland and porting
trees are intentionally not presented as supported standalone projects.

## Development principles

- Share behavior across architectures whenever hardware requirements permit.
- Keep architecture-specific entry and context code small and explicit.
- Validate both x86_64 and ARM64 before calling a cross-architecture change
  complete.
- Preserve clear boundaries between kernel source, development tooling, and
  distribution artifacts.
- Publish only source and reproducible metadata, never local VM state or build
  products.

EdgeOS Project source is distributed under the Mozilla Public License 2.0
unless a component states another compatible license.

