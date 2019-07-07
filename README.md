# fedora-workstation

Custom role to install fedora workstation for my use case.

The role will setup GNOME with a few extensions (including one from COPR build by myself), firefox with H264 support, some developper utilities and the NordVPN client configuration files.

## Role Variables

fedora_workstation_users: list of user to create. Those users will be part of the wheel group, and their dotfiles retrieve from github.com/<user>/dotfiles.


## Example Playbook

```
- hosts: localhost
  roles:
    - role: fedora-workstation
      vars:
        fedora_workstation_users:
          - jbertozzi
```

## License

BSD

## Author Information

Jeremy Bertozzi <jeremy.bertozzi@gmail.com>
