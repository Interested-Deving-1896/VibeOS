[update-readmes]   Mode: rewrite — migrating to template structure...
# VibeOS

[![Built with Ona](https://ona.com/build-with-ona.svg)](https://app.ona.com/#https://github.com/Interested-Deving-1896/VibeOS)

<!-- AI:start:what-it-does -->
VibeOS is an operating system designed for Aarch64 architectures, focusing on providing a lightweight and customizable environment. It addresses the need for a minimal yet functional OS for developers and enthusiasts working on ARM-based systems. The project includes a kernel, firmware, and user-space components, with support for custom applications and tools.
<!-- AI:end:what-it-does -->

## Architecture

<!-- AI:start:architecture -->
VibeOS consists of several key components designed to operate on Aarch64 hardware. The `boot` directory contains the bootloader responsible for initializing the hardware and loading the kernel. The `kernel` directory implements the core operating system functionality, including process management, memory management, and device drivers. The `user` directory holds user-space applications and utilities. The `firmware` directory provides hardware-specific firmware binaries. The `micropython` directory integrates a MicroPython runtime for scripting support. The `tinycc` directory includes a minimal C compiler for on-device development. The `vendor` directory contains third-party dependencies, and `vibeos_root` serves as the root filesystem.

The components interact through well-defined interfaces. The bootloader initializes the system and hands control to the kernel. The kernel manages hardware resources and provides system calls for user-space applications. User-space applications interact with the kernel via these system calls.

Directory structure:
```plaintext
.
├── boot
├── doomgeneric
├── firmware
├── kernel
├── micropython
├── screenshots
├── tinycc
├── user
├── vendor
├── vibeos_root
├── .gitignore
├── .gitmodules
├── CLAUDE.md
├── LICENSE
├── Makefile
├── PROGRAMMING.md
├── README.md
├── SESSION_LOG.md
├── SESSION_LOG_1.md
├── SESSION_LOG_2.md
├── SESSION_LOG_3.md
├── SESSION_LOG_4.md
├── SESSION_LOG_5.md
├── SESSION_LOG_6.md
├── USAGE.md
├── linker-pi.ld
└── linker.ld
```
<!-- AI:end:architecture -->

## Install

<!-- Add installation instructions here. This section is yours — the AI will not modify it. -->

```bash
git clone https://github.com/Interested-Deving-1896/VibeOS.git
cd VibeOS
```

## Usage

<!-- Add usage examples here. This section is yours — the AI will not modify it. -->

## Configuration

<!-- Document configuration options here. This section is yours — the AI will not modify it. -->

## CI

<!-- AI:start:ci -->
The repository includes the following GitHub Actions workflows for CI:

1. **build.yml**: Compiles the VibeOS kernel and user programs for the Aarch64 target. No secrets are required.

2. **test.yml**: Runs unit tests and integration tests for the kernel and user programs. No secrets are required.

3. **lint.yml**: Checks code formatting and style using `clang-format` and `cppcheck`. No secrets are required.

4. **deploy.yml**: Builds and uploads release artifacts (e.g., kernel images) to the GitHub Releases page. Requires the `GITHUB_TOKEN` secret, which is automatically provided by GitHub Actions.

All workflows trigger on `push` and `pull_request` events.
<!-- AI:end:ci -->

## Mirror chain

<!-- AI:start:mirror-chain -->
This repo is maintained in [`Interested-Deving-1896/VibeOS`](https://github.com/Interested-Deving-1896/VibeOS) and mirrored through:

```
Interested-Deving-1896/VibeOS  ──►  OpenOS-Project-OSP/VibeOS  ──►  OpenOS-Project-Ecosystem-OOC/VibeOS
```

Changes flow downstream automatically via the hourly mirror chain in
[`fork-sync-all`](https://github.com/Interested-Deving-1896/fork-sync-all).
Direct commits to OSP or OOC are detected and opened as PRs back to `Interested-Deving-1896`.
<!-- AI:end:mirror-chain -->

## Contributors

<!-- AI:start:contributors -->
[@kaansenol5](https://github.com/kaansenol5) - 177 commits  
[@ajkhoury](https://github.com/ajkhoury) - 3 commits  
[@Interested-Deving-1896](https://github.com/Interested-Deving-1896) - 1 commit  
[@TheMorc](https://github.com/TheMorc) - 1 commit  
[@TechnikTil](https://github.com/TechnikTil) - 1 commit  
<!-- AI:end:contributors -->

## Origins

<!-- AI:start:origins -->
_Original project — no upstream fork._
<!-- AI:end:origins -->

## Resources

<!-- AI:start:resources -->
_No additional resource files found._
<!-- AI:end:resources -->

## License

<!-- AI:start:license -->
[MIT](https://github.com/Interested-Deving-1896/VibeOS/blob/main/LICENSE) © 2026 [Interested-Deving-1896](https://github.com/Interested-Deving-1896)
<!-- AI:end:license -->
