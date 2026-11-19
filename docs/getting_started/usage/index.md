---
layout: default
title: Usage
parent: Getting Started
nav_order: 2
---

# Usage

```batch
Usage: winnvm [OPTIONS]

Options:

    -i, --install <version>    To install a new version of NodeJS
    -l, --list                 To list all installed versions of NodeJS
    -u, --use <version>        To use the given version of NodeJS
    -r, --remove <version>     To uninstall a version of NodeJS
    -h, --help                 Show this message
    -v, --version              Display Version
```

Only one command option can be specified per invocation. Options also accept `/` prefixes (e.g., `/i`, `/list`) and inline values (`--install=20.11.0`, `--install:20.11.0`, or `-i20.11.0`). A leading `v` in the version (such as `v20.11.0`) is optional.

## Install a Version of Node.js

Download and install a specific version of Node.js. WinNvm verifies the archive's SHA256 checksum against `SHASUMS256.txt` before extracting it into `NVM_HOME`.

```batch
winnvm -i <version>
```

or

```batch
winnvm --install <version>
```

## List Installed Versions of Node.js

List all Node.js versions installed in `NVM_HOME`, sorted by semantic version. The currently active version is marked with `*` and `(active)`.

```batch
winnvm -l
```

or

```batch
winnvm --list
```

## Use an Installed Version of Node.js

Switch the active Node.js version by pointing `NVM_SYMLINK` to the selected version using a Windows directory junction (`mklink /J`).

```batch
winnvm -u <version>
```

or

```batch
winnvm --use <version>
```

## Uninstall a Version of Node.js

Remove an installed version of Node.js from `NVM_HOME`. If the target version is currently active, switch to another version with `--use` before removing it.

```batch
winnvm -r <version>
```

or

```batch
winnvm --remove <version>
```
