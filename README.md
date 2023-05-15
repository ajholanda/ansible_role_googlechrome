# Ansible role googlechrome

Yet another Ansible role to install Google Chrome

## Requirements

None.

## Role Variables

- `googlechrome_linux_signing_key_url`:  GPG key for Linux systems.
- `googlechrome_yum_repository_url`: Yum repository.
- `googlechrome_apt_repository_url`: Apt repository to add in the sources list.
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
