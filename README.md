# fedora-workstation

Custom role to install fedora workstation for my use case.

The role will setup GNOME with a few extensions (including one from COPR build by myself), firefox with H264 support, some developper utilities and the NordVPN client configuration files.

## Role Variables

fedora_workstation_user: user to create. This user will be part of the wheel group, and its dotfiles retrieved from github.com/<user>/dotfiles.


## Example Playbook

```
- hosts: localhost
  roles:
    - role: fedora-workstation
      vars:
        fedora_workstation_user: jbertozzi
```

## License

BSD

## Author Information

Jeremy Bertozzi <jeremy.bertozzi@gmail.com>
