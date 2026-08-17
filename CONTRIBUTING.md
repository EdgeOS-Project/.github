# Contributing to EdgeOS Project

Thank you for helping improve EdgeOS. Keep each change focused, explain its
user-visible or kernel-visible effect, and include the validation that was run.

For cross-architecture kernel changes:

- put shared behavior in shared code;
- retain separate code only for required architecture entry, context, or
  hardware behavior;
- run the repository's ABI inventory and architecture-unity checks; and
- build both x86_64 and ARM64.

For Workstation changes, run the Python compilation and regression commands in
that repository's contributing guide.

Do not include credentials, local paths, VM images, generated build products,
or test data containing personal information.

