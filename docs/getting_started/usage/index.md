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

    -i, --install <verison>    To install a new version of NodeJS
    -u, --use <version>        To use the given version of NodeJS
    -r, --remove <version>     To uninstall a version of NodeJS
    -h, --help                 Show this message
    -v, --version              Display Version
```

## Install a version of NodeJS.

To install a version a NodeJS use the following command where `<version>` is the version of the NodeJS.

```batch
winnvm -i <version>
```

or

```batch
winnvm --install <version>
```

## To use a installed NodeJS.

To use an already installed NodeJS version use the following command where `<version>` is the version of the NodeJS.

```batch
winnvm -u <version>
```

or

```batch
winnvm --use <version>
```

## To uninstall a verson of NodeJS.

To remove/uninstall an installed version of NodeJS use the following command where `<version>` is the version of the NodeJS.

```batch
winnvm -r <version>
```

or

```batch
winnvm --remove <version>
```
