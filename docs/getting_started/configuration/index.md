---
layout: default
title: Configuration
parent: Getting Started
nav_order: 3
---

# Configuration

## `.winnvmrc`

WinNvm reads optional configuration from `%USERPROFILE%\.winnvmrc` in JSON format.

```json
{
  "nodemirror": "https://nodejs.org/dist/"
}
```

| Property     | Default                    | Description                                                                 |
|--------------|----------------------------|-----------------------------------------------------------------------------|
| `nodemirror` | `https://nodejs.org/dist/` | Base URL of the Node.js distribution mirror (a trailing `/` is added if omitted). |

Property names are matched case-insensitively.

## Environment Variables

| Variable      | Description                                                                 |
|---------------|-----------------------------------------------------------------------------|
| `NVM_HOME`    | Directory where downloaded Node.js versions (`v<version>`) are stored.      |
| `NVM_SYMLINK` | Directory junction path pointing to the currently active Node.js version.   |
