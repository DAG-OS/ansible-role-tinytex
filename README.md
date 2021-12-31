# TinyTeX

A role for installing TinyTeX in a multi-user setup.

## Requirements

Root privileges are required for a successful installation.

## Role Variables

* `state`: Defines the state this roles aims to achieve, defaults to `present`. One of the following:
  * `present`: Ensures TinyTeX is installed.
  * `install`: Ensures TinyTeX is installed.
  * `latest`: Ensures TinyTeX is installed and updated.
  * `absent`: Removes the TinyTeX installation.
* `install_dir`: A path where TinyTeX should be installed, defaults to `/opt/tinytex`
* `packages`: A list of packages to install

## Dependencies

None.

## Example Playbook

The most basic usage:

```yaml
- name: Ensure TinyTeX is installed
  hosts: all
  roles:
    - role: dagos.tinytex
```
