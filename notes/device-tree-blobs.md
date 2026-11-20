# QEMU Environment Setup

## Part 1: Build Dependencies

Before Cloning the Source Code of QEMU Commands Ran:
```bash
sudo apt update
sudo apt install -y git libglib2.0-dev libfdt-dev libpixman-1-dev zlib1g-dev ninja-build build-essential python3

**apt update:** Refreshes Local Packages.

**git:** Version control.

**libglib2.0-dev:** Development headers and libraries for GLib, QEMU's foundational C utility library providing main loops, data structures, threads, error handling, and object/event infrastructure.

**libfdt-dev:** Development headers and static/shared library for libfdt (Flattened Device Tree), used by QEMU to create, read, and dynamically modify Device Tree blobs passed to guest kernels.

**libpixman-1-dev:** Pixel manipulation library supporting low-level 2D image compositing and region operations used by QEMU display/framebuffer and graphics emulation paths.

**zlib1g-dev:** Compression library headers used for compressed data streams, snapshot/migration or archive handling, and related utilities within QEMU.

**ninja-build:** Fast build executor (ninja) invoked after Meson/QEMU generates build targets; handles incremental recompilation quickly during iterative development.

**build-essential:** Meta-package providing core compilation tools (gcc, g++, make, libc6-dev, etc.) required to compile C/C++ code.

**python3:** Used heavily throughout QEMU's build system, code generators, QAPI/schema tooling, and test scripts.


## Device Tree Blob 
