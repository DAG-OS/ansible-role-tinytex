# LaTeX

A role for installing LaTeX.

## Requirements

When choosing the TeXLive vendor as installation option root privileges are required.

## Role Variables

- `state`: Either `present` or `install`
- `vendor`: Either `tinytex` or `texlive`
- `packages`: A list of packages to install

## Dependencies

None.

## Example Playbook

```yaml
- name: Install LaTeX
  hosts: all
  roles:
    - role: dagos.latex
      vars:
        state: present
        vendor: tinytex
```
