---
title: Options and Configuration
layout: default
grand_parent: Releases
parent: v1.0.0
nav_order: 2
---

## Options

### Help
To see the help information use `winnvm -h`.

### Installing new NodeJS version.
To install new version of NodeJS use `winnvm -i <version>`.

### Switching Node Versions
To switch to a NodeJs version use `winnvm -u <version>`.

## Configuration
The configurations for winnvm are stored in `%USER_HOME%\.winnvmrc` which is a json format file. Currently only one configuration is the
```javascript
{
    nodemirror:'<url of the mirror>'
}
```
