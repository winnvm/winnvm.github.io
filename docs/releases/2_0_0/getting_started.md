---
title: Getting Started
layout: default
grand_parent: Releases
parent: v2.0.0
nav_order: 1
---

## Prerequisites

- Windows (x64 or ARM64). No separate .NET runtime is required for release binaries.

## Installation

### MSI Installer (Recommended)

Download the MSI installer for your architecture (`win-x64` or `win-arm64`) from [GitHub Releases](https://github.com/winnvm/winnvm/releases) and run it. The installer sets `NVM_HOME` (default `%LocalAppData%\WinNvm`), `NVM_SYMLINK` (default `%LocalAppData%\nodejs`), and updates your user `PATH` automatically.

### Portable ZIP / Standalone Executable

1. Download the `.zip` or `.exe` asset from [GitHub Releases](https://github.com/winnvm/winnvm/releases), extract it to a folder, and add that folder to `PATH`.
2. Set `NVM_HOME` and `NVM_SYMLINK` user environment variables, and add `%NVM_SYMLINK%` to `PATH`.

## Testing the Installation

Open a Command Prompt or PowerShell window and run:

```batch
winnvm -v
```
