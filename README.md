# TinyTeX

A role for installing TinyTeX in a multi-user setup.

## Requirements

Root privileges are required for a successful installation.

## Role Variables

- `state`: Either `present` or `install`
- `install_dir`: A path where TinyTeX should be installed
- `packages`: A list of packages to install

## Dependencies

None.

## Example Playbook

```yaml
- name: Install LaTeX
  hosts: all
  roles:
    - role: dagos.tinytex
      vars:
        state: present
```
