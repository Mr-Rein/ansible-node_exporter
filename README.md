# Node_exporter ansible setup

Simple role to setup node_exporter. This has only been tested on:

- `AlmaLinux 9.0`
- `AlmaLinux 9.1`
- `Debian 11.5`
- `Debian 11.6 - aarch64 (ARM)`

## Requirements

Minimum `AlmaLinux 9.0` or `Debian 11.5` node.

## Role Variables

The variables are defined in `defaults/main.yml`. These should be configured as needed:

- `packages`
- `exporter_user`
- `exporter_download_location`
- `exporter_version`

## Example playbook

```yml
---
- name: test playbook
  hosts: general

  roles:
  - role: ansible-node_exporter
```
