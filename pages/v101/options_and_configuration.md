---
title: Options and Configuration
sidebar: winnvm_101_sidebar
permalink: /v101/options_and_configuration.html
---

## Options

### Help
To see the help information use `winnvm -h`.

### Installing new NodeJS version.
To install new version of NodeJS use `winnvm -i <version>`.

### Switching Node Versions
To switch to a NodeJs version use `winnvm -u <version>`.

### Uninstalling a Node Version
To uninstall a NodeJS version use `winnvm -r <version>`.

## Configuration
The configurations for winnvm are stored in `%USER_HOME%\.winnvmrc` which is a json format file. Currently only one configuration is the
```json
{
    nodemirror:url of the mirror.
}
```

{% include links.html %}
