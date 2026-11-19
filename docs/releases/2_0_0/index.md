---
layout: default
title: v2.0.0
parent: Releases
nav_order: 96
has_children: true
---

# Release Notes

In this release, WinNvm has been modernized to .NET 10 with self-contained builds, Windows ARM64 support, and an MSI installer:

1. **Upgraded to .NET 10 (`net10.0`):** Published as self-contained single-file executables (`--self-contained`) — no separate .NET Framework or .NET runtime installation is required.
2. **Windows ARM64 & x64 Support:** Release builds target both `win-x64` and `win-arm64`, and Node.js downloads automatically match the host architecture (`arm64`, `x64`, or `x86`).
3. **Per-User MSI Installer:** Added WiX-based MSI installers (`WinNvm-<version>-win-x64.msi` and `WinNvm-<version>-win-arm64.msi`) with interactive `NVM_HOME` / `NVM_SYMLINK` configuration, automatic user `PATH` setup, and silent `msiexec` support.
4. **SHA256 Verification & Safe Extraction:** Verifies downloaded Node.js archives against `SHASUMS256.txt` and extracts via a temporary staging directory with path-traversal protection.
5. **Improved `-l` / `--list` Output:** Lists installed versions sorted by semantic version and highlights the active version (`* <version> (active)`).
6. **Active Version Guard on Removal:** Prevents `-r` / `--remove` from deleting the currently active Node.js version until you switch with `--use`.
7. **Flexible CLI Option Parsing:** Supports `-`, `--`, and `/` prefixes as well as inline values (`--install=20.11.0`, `--install:20.11.0`, `-i20.11.0`) and optional `v` prefixes on version numbers.
