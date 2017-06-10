# Ansible role 'desktop'

An Ansible role for setting up something for whatever purpose.

## Requirements

## Role Variables
`foopkg` (`true|false`) declares whether package groups are to be installed.

| Variable                       | Default                          | Comments (type)  |
| :---                           | :---                             | :---             |
|`xorgpkg`| `true` ||
|`latexpkg`| `true` ||
|`kdepkg`| `true`||
|`i3pkg`| `true`||
|`mediapkg`| `true`||
|`appearancepkg`| `true`||
|`toolspkg`| `true`||
|`browserspkg`| `true`||
|`desktoppkg`| `true`||
|`networkpkg`| `true`||
|`officepkg`| `true`||
|`createpkg`| `true`||
|`i3user`| splatrat||
|`i3group`| splatrat||


## Dependencies
No playbook dependencies, but for Arch Linux pacaur needs to be installed along with a pacaur module, such as
Austin Hyde's.

## Example Playbook
```Yaml
- hosts: foo
  roles:
    - role: desktop
```

## Testing

## License

BSD

## Contributors

Issues, feature requests, ideas, suggestions, etc. are appreciated and can be posted in the Issues section. Pull requests are also very welcome. Please create a topic branch for your proposed changes, it's the easiest way to merge back into the project.

- [Oscar Petersson](https://giithub.com/oscpe262/) (Maintainer)
