# Ansible role 'ansible-role-plexserver'

An Ansible role for setting up a Plex Media Server.

## Requirements
This role has been developed for Fedora 27. No guarantees provided for any other distro, but should be applicable to most of the common ones. The defaults are for Fedora, and it will modify the plex account to access all media available to users in the group "users". 

## Role Variables
| Variable		| Default		| Comments (type) |
| :---			| :---			| :---		  |
| `plex_url` | RPM URL | This defaults to a rpm url, but can be replaced with a package name if available in some enabled repo. |
| `plex_group` | `users` | Additional groups to give plex user access to. Comma-separated list. |

## Dependencies

## Example Playbook
```Yaml
- hosts: foo
  roles:
    - role: ansible-role-plexserver
```

## Testing


## License

BSD

## Contributors

Issues, feature requests, ideas, suggestions, etc. are appreciated and can be posted in the Issues section. Pull requests are also very welcome. Please create a topic branch for your proposed changes, it's the easiest way to merge back into the project.

- [Oscar Petersson](https://github.com/oscpe262/) (Maintainer)
