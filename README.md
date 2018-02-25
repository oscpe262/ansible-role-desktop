# Ansible role 'desktop'

An Ansible role for setting up desktop environments. What to include is in this kind of role is of course
highly subjective, but I've included what I use and have tried to keep it as modular as possible. Suggestions
to how to improve is always welcome.

TODO: Re-check Fedora packages to make it equivalent to Arch.

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
|`i3user`| foo ||
|`i3group`| users ||
|`laptop` | `false` | set to true for laptops, will provide battery info etc. |
| `maincolor` | B5BD56 | Hex color value, for i3 |
| `wlp` | wlp58s0 | wireless device name |

## Dependencies
No playbook dependencies, but for Arch Linux pacaur needs to be installed along with a pacaur module, such as
Austin Hyde's.
For Fedora, rpm-fusion repos are required for default usage.

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

- [Oscar Petersson](https://github.com/oscpe262/) (Maintainer)
