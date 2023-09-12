# Common vm configuration

This is a role to set up machines in a general environment.

This role assumes that the machine has only one network interface.

## Requirements

- Ansible
- root access
- network interface config
- hostname

## Role Variables

There are NO default values in this role! If a variable file in ```host_vars``` or command line variables are not set up properly, the role must and will fail!

```
common_interface: enp0s3
common_ip: 1.2.3.4
common_gateway: 4.5.6.7
common_hostname: ansiserver
common_install:
  - vim
  - tmux
  - python3
```

## Dependencies

- ansible >= 2.10

## Example Playbook


    - hosts: all
      roles:
         - role: common

## License

MIT

## Author Information

Tamas Molnar - <tmolnar0831@gmail.com> - https://tomsitcafe.com
