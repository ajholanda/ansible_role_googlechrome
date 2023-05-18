# Ansible role googlechrome

Yet another Ansible role to manage Google Chrome installation

## Requirements

None.

## Role Variables

- `package_state`: et a default value that can be used as a global variable across roles [ajholanda roles](https://galaxy.ansible.com/ajholanda). 
- `googlechrome_linux_signing_key_url`: GPG key for Linux systems.
- `googlechrome_yum_repository_url`: yum repository.
- `googlechrome_apt_repository_url`: apt repository to add in the sources list.
- `googlechrome_state`: desired state after running package manager task.

## Dependencies

None.

## Example Playbook

```
    - hosts: all
      roles:
        - ajholanda.googlechrome
```

To uninstall

```
    - hosts: all
      vars:
        googlechrome_state: absent
      roles:
        - ajholanda.googlechrome
```
## License

MIT.

## Author Information

[Adriano J. Holanda](https://ajholanda.github.io).
