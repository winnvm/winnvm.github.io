---
layout: default
title: Installation
parent: Getting Started
nav_order: 1
---
# Installation

## Prerequisite

Windows with .NET Framework 4.8 or later.

## Steps.

1. Download the latest version from [GitHub][download].
2. Extract to a folder.
3. Add the extracted folder to path.
4. Create the following Enviroment variables.

    | Variable      | Description                                                                 |
    |---------------|-----------------------------------------------------------------------------|
    | `NVM_HOME`    | This should be a folder name which already exists.                          |
    | `NVM_SYMLINK` | This should also be a folder name but only the parent folder should exists. |

    Add `NVM_SYMLINK` to the `PATH` variable

## Testing the installation.
Open command prompt and try `winnvm -v` which should print the version.

[download]:https://github.com/winnvm/winnvm/releases/download/v1.0.3/WinNvm-v1.0.3.zip
