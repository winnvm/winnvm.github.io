---
layout: default
title: Installation
parent: Getting Started
nav_order: 1
---
# Installation

## Prerequisites

- **OS:** Windows (x64 or ARM64)
- **Runtime:** None required for release binaries (published as self-contained single-file executables).
  - *If building from source:* [.NET 10 SDK](https://dotnet.microsoft.com/download/dotnet/10.0) (and WiX Toolset v5 if building the MSI installer).

## Option 1: MSI Installer (Recommended)

1. Download the MSI installer for your architecture from the [GitHub Releases][releases] page:
   - `WinNvm-<version>-win-x64.msi` (64-bit Intel/AMD)
   - `WinNvm-<version>-win-arm64.msi` (64-bit ARM)
2. Run the installer. It performs a per-user installation (no administrator privileges required) and lets you configure:
   - **Install folder** (default: `%LocalAppData%\WinNvm`)
   - **`NVM_HOME`** — directory where Node.js versions are stored (default: `%LocalAppData%\WinNvm`)
   - **`NVM_SYMLINK`** — directory junction for the active Node.js version (default: `%LocalAppData%\nodejs`)
3. The installer automatically sets `NVM_HOME` and `NVM_SYMLINK` and adds the install folder, `NVM_HOME`, and `NVM_SYMLINK` to your user `PATH`.

### Silent MSI Installation

You can also install silently via `msiexec` and override `NVM_HOME` or `NVM_SYMLINK`:

```batch
msiexec /i WinNvm-v2.0.0-win-x64.msi /qn NVM_HOME="C:\Tools\winnvm" NVM_SYMLINK="C:\Tools\nodejs"
```

## Option 2: Portable ZIP / Standalone Executable

1. Download the `.zip` archive (or standalone `.exe`) for your architecture (`win-x64` or `win-arm64`) from [GitHub Releases][releases].
2. Extract `WinNvm.exe` to a folder of your choice and add that folder to your `PATH`.
3. Create the following user environment variables:

   | Variable      | Description                                                               |
   |---------------|---------------------------------------------------------------------------|
   | `NVM_HOME`    | Directory where Node.js versions will be stored (created automatically if missing). |
   | `NVM_SYMLINK` | Path for the active Node.js directory junction (parent directory should exist). |

4. Add `%NVM_SYMLINK%` to your `PATH` environment variable.

## Testing the Installation

Open a new Command Prompt or PowerShell window and run:

```batch
winnvm -v
```

This should print the installed `WinNvm` version.

[releases]: https://github.com/winnvm/winnvm/releases
