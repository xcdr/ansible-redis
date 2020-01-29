# Ansible role for Redis

This is a simple Ansible role for installing Redis via ansible-galaxy.

The role should work on all Debian based distributions.

## Installation

Add this to your `requirements.yml`:

```yml
- src: https://github.com/xcdr/ansible-redis
  name: xcdr.redis
```

## Example playbook

```yaml
---

- hosts: myhost
  roles: xcdr.redis

  vars:
    redis_params:
    - key: "bind"
      value: "0.0.0.0"
```

## License

MIT
