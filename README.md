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
* `ssh_server_windows_adminauthorizedkeys`: content of the `administrators_authorized_keys` file (default: nil)
  * **Note**: it is recommended to use a `|` operator to set multiline contents, such as:
  ```
  ssh_server_windows_adminauthorizedkeys: |
    somekey
    someotherkey
    [...]
  ```

# License

Apache-2.0
