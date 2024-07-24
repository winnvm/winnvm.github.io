---
title: Getting Started
layout: default
grand_parent: Releases
parent: v1.0.1
nav_order: 1
---

## Prerequisite
1. Windows with .NET Framework 4 or later.

## Environment Variables.
The following environment variables should be present.

1. `NVM_HOME` -> This should be a folder name which already exists.
2. `NVM_SYMLINK` -> This should also be a folder name but only the parent folder should exists.

Add `NVM_SYMLINK` to you `PATH`

## Installation
Download [WinNvm](https://github.com/winnvm/winnvm/releases/download/v1.0.1/WinNvm_v1.0.1.zip) and extract to a folder. Add the extracted folder to path.

## Testing the installation.
Open command prompt and try `winnvm -v` which should print the version.
