# nvm

[![Build Status](https://img.shields.io/travis/fanatid/ansible-role-nvm.svg?branch=master&style=flat-square)](https://travis-ci.org/fanatid/ansible-role-nvm)

## Requirements

git, build-essential, libssl-dev

## Role Variables

  - `nvm.user` Remote user. Default value is `ansible_user`.
  - `nvm.version` NVM version tag, or HEAD. Default is `v0.33.0`.
  - `nvm.node_version` Node.js version. Default is `6.5.0`.

## Dependencies

No depedencies.

## Example Playbook

```
- hosts: servers
  roles:
    - role: nvm
      nvm:
        user: deploy
        version: v0.33.0
        node_version: '7.0.0'
```

## LICENSE

This library is free and open-source software released under the MIT license.
