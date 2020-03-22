# loumaris.ssh-hardening

Some ssh default settings like no root login.

## usage

Example entry for the `playbook.yml`

```yaml
- name: apply common configuration to all nodes
  hosts: all
  roles:
    - loumaris.ssh-hardening
```

## configuration

You need to set the following parameter (in the vault):
* `sshd` (name of the ssh service (default is _ssh_))
* `sshd_config` (path to sshd config (default is _/etc/ssh/sshd_config_))