# Ansible Role for Molecule

[![Gitlab pipeline status](https://img.shields.io/gitlab/pipeline/alvistack/ansible-role-molecule/master)](https://gitlab.com/alvistack/ansible-role-molecule/-/pipelines)
[![GitHub release](https://img.shields.io/github/release/alvistack/ansible-role-molecule.svg)](https://github.com/alvistack/ansible-role-molecule/releases)
[![GitHub license](https://img.shields.io/github/license/alvistack/ansible-role-molecule.svg)](https://github.com/alvistack/ansible-role-molecule/blob/master/LICENSE)
[![Ansible Role](https://img.shields.io/badge/galaxy-alvistack.molecule-blue.svg)](https://galaxy.ansible.com/alvistack/molecule)

Ansible Role for Molecule Installation (what the hell is this\!?).

[Molecule 3.1.1+](https://github.com/ansible-community/molecule/releases/tag/3.1.1) only keep [Delegated Driver](https://molecule.readthedocs.io/en/latest/configuration.html#delegated) in core, therefore additional drivers support (e.g. docker, podman, vagrant, etc) and corresponding dependencies should be handled manually.

Following Molecule drivers are supported by this role:

  - [Molecule Docker](https://github.com/ansible-community/molecule-docker)
  - [Molecule Vagrant](https://github.com/ansible-community/molecule-vagrant)

## Requirements

This role require Ansible 2.10 or higher.

This role was designed for:

  - Ubuntu 18.04, 20.04, 20.10, 21.04
  - CentOS 7, 8 Stream
  - openSUSE Leap 15.2, Tumbleweed
  - Debian 10
  - Fedora 33
  - RHEL 7, 8

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
