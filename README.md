# Ansible Role: BasslineMnk

[![CircleCI](https://circleci.com/gh/bassline-mnk/ansible-role-basslinemnk.svg?style=svg)](https://circleci.com/gh/bassline-mnk/ansible-role-basslinemnk)
[![License](http://img.shields.io/:license-mit-blue.svg?style=flat-square)](LICENSE)

Ansible role for [BasslineMnk KVM](https://github.com/bassline-mnk/basslinemnk).

## Role Variables

Available variables are listed below, along with default values (see [defaults/main.yml](defaults/main.yml)):

```yaml
basslinemnk_group: basslinemnk
basslinemnk_dir: /opt/basslinemnk
basslinemnk_repo: https://github.com/bassline-mnk/basslinemnk.git
basslinemnk_repo_branch: master
basslinemnk_interface: '127.0.0.1'
basslinemnk_port: 8000
basslinemnk_keyboard_interface: /dev/hidg0
```

## Dependencies

* [bassline-mnk.ustreamer](https://github.com/bassline-mnk/ansible-role-ustreamer)
* [bassline-mnk.nginx](https://github.com/bassline-mnk/ansible-role-nginx)

## Example Playbook

#### `example.yml`

```yaml
- hosts: all
  roles:
    - role: ansible-role-basslinemnk
```

### Running Example Playbook

```bash
ansible-galaxy install git+https://github.com/bassline-mnk/ansible-role-basslinemnk.git
ansible-playbook example.yml
```

## License

MIT

## Author Information

This role was created in 2020 by [Adrian Griffin](http://adrian-griffin.io).
