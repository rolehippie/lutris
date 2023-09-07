# lutris

[![Source Code](https://img.shields.io/badge/github-source%20code-blue?logo=github&logoColor=white)](https://github.com/rolehippie/lutris)
[![General Workflow](https://github.com/rolehippie/lutris/actions/workflows/general.yml/badge.svg)](https://github.com/rolehippie/lutris/actions/workflows/general.yml)
[![Readme Workflow](https://github.com/rolehippie/lutris/actions/workflows/docs.yml/badge.svg)](https://github.com/rolehippie/lutris/actions/workflows/docs.yml)
[![Galaxy Workflow](https://github.com/rolehippie/lutris/actions/workflows/galaxy.yml/badge.svg)](https://github.com/rolehippie/lutris/actions/workflows/galaxy.yml)
[![License: Apache-2.0](https://img.shields.io/github/license/rolehippie/lutris)](https://github.com/rolehippie/lutris/blob/master/LICENSE)
[![Ansible Role](https://img.shields.io/badge/role-rolehippie.lutris-blue)](https://galaxy.ansible.com/rolehippie/lutris)

> [!IMPORTANT]
> This role have been archived because of the lack of maintenance and because
> we are not actively using it anymore. If you are using this role feel free
> to fork and maintain it on your own. Maybe we will unarchive this repository
> in the future at some point, maybe not... Who knows...

Ansible role to install lutris gaming platform.

## Sponsor

Building and improving this Ansible role have been sponsored by my current and previous employers like **[Cloudpunks GmbH](https://cloudpunks.de)** and **[Proact Deutschland GmbH](https://www.proact.eu)**.

## Table of content

- [Requirements](#requirements)
- [Default Variables](#default-variables)
  - [lutris_dependencies](#lutris_dependencies)
  - [lutris_package](#lutris_package)
  - [lutris_version](#lutris_version)
- [Discovered Tags](#discovered-tags)
- [Dependencies](#dependencies)
- [License](#license)
- [Author](#author)

---

## Requirements

- Minimum Ansible version: `2.10`

## Default Variables

### lutris_dependencies

List of packages required by lutris

#### Default value

```YAML
lutris_dependencies:
  - wine64
  - wine32
  - libasound2-plugins:i386
  - libsdl2-2.0-0:i386
  - libdbus-1-3:i386
  - libsqlite3-0:i386
```

### lutris_package

Download URL for the package to install

#### Default value

```YAML
lutris_package: https://github.com/lutris/lutris/releases/download/v{{ lutris_version
  }}/lutris_{{ lutris_version }}_all.deb
```

### lutris_version

Version for the package

#### Default value

```YAML
lutris_version: 0.5.13
```

## Discovered Tags

**_lutris_**


## Dependencies

- None

## License

Apache-2.0

## Author

[Thomas Boerger](https://github.com/tboerger)
