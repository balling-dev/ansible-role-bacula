# bacula

Install and configure [bacula](https://www.bacula.org/) - a set of computer
programs that permit managing backup, recovery, and verification of computer
data across a network of computers of different kinds.

|GitHub|Downloads|Version|
|------|---------|-------|
|[![github](https://github.com/balling-dev/ansible-role-bacula/workflows/Continuous%20Integration/badge.svg)](https://github.com/balling-dev/ansible-role-bacula/actions)|[![downloads](https://img.shields.io/ansible/role/d/balling-dev/bacula)](https://galaxy.ansible.com/ui/standalone/roles/balling-dev/bacula)|[![Version](https://img.shields.io/github/release/balling-dev/ansible-role-bacula.svg)](https://github.com/balling-dev/ansible-role-bacula/releases/)|

## Example Playbook

This example is taken from
[`molecule/default/converge.yml`](
https://github.com/balling-dev/ansible-role-bacula/blob/main/molecule/default/converge.yml)
and is tested on each push, pull request and release.

```yaml
---
- name: "Converge"
  hosts: "all"
  become: true
  gather_facts: true

  roles:
    - role: "balling-dev.bacula"
```

## Role Variables

The default values for the variables are set in
[`defaults/main.yml`](https://github.com/balling-dev/ansible-role-bacula/blob/main/defaults/main.yml):

```yaml
---
# Defaults file for bacula

# Version of bacula to install. Use "latest" to install latest version.
bacula_version: "latest"
```
