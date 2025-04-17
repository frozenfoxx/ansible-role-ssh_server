# ansible-role-ssh_server

Ansible role to set up OpenSSH.

# Requirements

## Windows
- Server 2022+

# Usage

```
- hosts: all
  roles:
    - { role: frozenfoxx.ssh_server }
```

# Variables

* `ssh_server_windows_disableadminauthkeys`: disables system-wide Administrators authorized keys file (default: `True`)

# License

Apache-2.0
