# Ansible Role for Molecule

<a href="https://alvistack.com" title="AlviStack" target="_blank"><img src="/alvistack.svg" height="75" alt="AlviStack"></a>

[![Gitlab pipeline status](https://img.shields.io/gitlab/pipeline/alvistack/ansible-role-molecule/master)](https://gitlab.com/alvistack/ansible-role-molecule/-/pipelines)
[![GitHub tag](https://img.shields.io/github/tag/alvistack/ansible-role-molecule.svg)](https://github.com/alvistack/ansible-role-molecule/tags)
[![GitHub license](https://img.shields.io/github/license/alvistack/ansible-role-molecule.svg)](https://github.com/alvistack/ansible-role-molecule/blob/master/LICENSE)
[![Ansible Role](https://img.shields.io/badge/galaxy-alvistack.molecule-blue.svg)](https://galaxy.ansible.com/alvistack/molecule)

Ansible Role for Molecule Installation (what the hell is this!?).

[Molecule 3.1.1+](https://github.com/ansible-community/molecule/tags/tag/3.1.1) only keep [Delegated Driver](https://molecule.readthedocs.io/en/latest/configuration.html#delegated) in core, therefore additional drivers support (e.g. docker, podman, vagrant, etc) and corresponding dependencies should be handled manually.

Following Molecule drivers are supported by this role:

- [Molecule Docker](https://github.com/ansible-community/molecule-docker)
- [Molecule Vagrant](https://github.com/ansible-community/molecule-vagrant)

## Requirements

This role require Ansible community package 4.10 or higher.

This role was designed for:

- Ubuntu 20.04, 22.04, 24.04, 24.10, 25.04
- AlmaLinux 8, 9
- openSUSE Leap 15.6, Tumbleweed
- Debian 12, Testing
- Fedora 41, 42, Rawhide
- CentOS 7, 8 Stream, 9 Stream
- RHEL 7, 8, 9

## Role Variables

[defaults/main.yml](defaults/main.yml)

## Dependencies

[ansible-galaxy-requirements.yml](ansible-galaxy-requirements.yml)

## Example Playbook

[molecule/default/converge.yml](molecule/default/converge.yml)

This role could simply deploy to `localhost` as below:

    molecule converge -s default

## License

- Code released under [Apache License 2.0](LICENSE)
- Docs released under [CC BY 4.0](http://creativecommons.org/licenses/by/4.0/)

## Author Information

- Wong Hoi Sing Edison
  - <https://twitter.com/hswong3i>
  - <https://github.com/hswong3i>
