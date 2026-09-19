# Caddy-Role

[![Alma9-CI](https://github.com/philnewm/ansible-caddy/actions/workflows/alma9-ci-caller.yml/badge.svg)](https://github.com/philnewm/ansible-caddy/actions/workflows/alma9-ci-caller.yml)  [![Rocky9-CI](https://github.com/philnewm/ansible-caddy/actions/workflows/rocky9-ci-caller.yml/badge.svg)](https://github.com/philnewm/ansible-caddy/actions/workflows/rocky9-ci-caller.yml)  [![CentOSStream9-CI](https://github.com/philnewm/ansible-caddy/actions/workflows/centosstream9-ci-caller.yml/badge.svg)](https://github.com/philnewm/ansible-caddy/actions/workflows/centosstream9-ci-caller.yml)  [![Debian13-CI](https://github.com/philnewm/ansible-caddy/actions/workflows/debian13-ci-caller.yml/badge.svg)](https://github.com/philnewm/ansible-caddy/actions/workflows/debian13-ci-caller.yml)  [![Ubuntu2404-CI](https://github.com/philnewm/ansible-caddy/actions/workflows/ubuntu2404-ci-caller.yml/badge.svg)](https://github.com/philnewm/ansible-caddy/actions/workflows/ubuntu2404-ci-caller.yml)

Role description

This role includes a vagrant based molecule testing setup as a submodule at `molecule/`

## Structure

```code
📦 ansible-caddy
 ┣ 📂defaults
 ┃ ┗ 📜main.yml
 ┣ 📂files
 ┃ ┗ 📜Caddyfile
 ┣ 📂meta
 ┃ ┗ 📜main.yml
 ┣ 📂 molecule
 ┃ ┗ 📂 default
 ┃   ┗ 📜, 📜, 📜, scenario_files
 ┣ 📂tasks
 ┃ ┣ 📜absent.yml
 ┃ ┣ 📜main.yml
 ┃ ┣ 📜present.yml
 ┃ ┣ 📜service_setup.yml
 ┃ ┗ 📜tests.yml
 ┣ 📂templates
 ┃ ┗ 📜caddy.container.j2
 ┣ 📂vars
 ┃ ┗ 📜main.yml
 ┣ 📜.gitignore
 ┣ 📜.gitmodules
 ┣ 📜README.md
 ┗ 📜requirements.yml

```

Describe and explain role structure.

## Requirements

Elaborate external dependencies and how to use them.

## Role Variables

* defaults/main.yml
  * first_var
  * sec_var
  * third_var
* vars/main.yml
  * first_var
  * sec_var
  * third_var

## Dependencies

List role ansible-galaxy dependencies - if any.

## Example Playbook

Add an example playbook

```yaml
---

tasks:
  - name: Include ansible-caddy present
    ansible.builtin.include_role:
      name: ansible-caddy
    vars:
      state: present

...
```

## License

Add license - if any.
