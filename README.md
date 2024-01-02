# starship

[![Source Code](https://img.shields.io/badge/github-source%20code-blue?logo=github&logoColor=white)](https://github.com/rolehippie/starship)
[![General Workflow](https://github.com/rolehippie/starship/actions/workflows/general.yml/badge.svg)](https://github.com/rolehippie/starship/actions/workflows/general.yml)
[![Readme Workflow](https://github.com/rolehippie/starship/actions/workflows/docs.yml/badge.svg)](https://github.com/rolehippie/starship/actions/workflows/docs.yml)
[![Galaxy Workflow](https://github.com/rolehippie/starship/actions/workflows/galaxy.yml/badge.svg)](https://github.com/rolehippie/starship/actions/workflows/galaxy.yml)
[![License: Apache-2.0](https://img.shields.io/github/license/rolehippie/starship)](https://github.com/rolehippie/starship/blob/master/LICENSE)
[![Ansible Role](https://img.shields.io/badge/role-rolehippie.starship-blue)](https://galaxy.ansible.com/rolehippie/starship)

Ansible role to install starship shell prompt.

## Sponsor

Building and improving this Ansible role have been sponsored by my current and previous employers like **[Cloudpunks GmbH](https://cloudpunks.de)** and **[Proact Deutschland GmbH](https://www.proact.eu)**.

## Table of content

- [Requirements](#requirements)
- [Default Variables](#default-variables)
  - [starship_arch](#starship_arch)
  - [starship_download](#starship_download)
  - [starship_version](#starship_version)
- [Discovered Tags](#discovered-tags)
- [Dependencies](#dependencies)
- [License](#license)
- [Author](#author)

---

## Requirements

- Minimum Ansible version: `2.10`

## Default Variables

### starship_arch

Architecture of the static binary

#### Default value

```YAML
starship_arch: '{{ ansible_architecture }}'
```

### starship_download

URL to the archive of the release to install

#### Default value

```YAML
starship_download: https://github.com/starship/starship/releases/download/v{{ starship_version
  }}/starship-{{ starship_arch }}-unknown-linux-musl.tar.gz
```

### starship_version

Version of the release to install

#### Default value

```YAML
starship_version: 1.17.1
```

## Discovered Tags

**_starship_**


## Dependencies

- [rolehippie.docker](https://github.com/rolehippie/docker)

## License

Apache-2.0

## Author

[Thomas Boerger](https://github.com/tboerger)
