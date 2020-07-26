# LDAPD configuration for OpenBSD

## Server side requirements:
- OpenBSD
- Python 3

## Role variables

| Variable | Default Value | Description |
| -------- | ------------- | ----------- |
| `ldap_domains` | [] | List of domains to configure for ldap. |
| `ldap_admin` | "root" | Top level user with access to everything. |
| `ldap_admin_pass` | "{BSDAUTH}root" | Method to authenticate the root user, defaults to using the inbuilt BASDAUTH OS login mechanism. |
| `ldap_uid_start` | 1000 | The starting point for UID. This value auto-increments for every user defined in `ldap_users`. |
| `ldap_gid_start` | 1000 | The starting point for GID. This also auto-increments. |

For a detailed description of all variables look at the file [defaults/main.yml](defaults/main.yml).

## Example configuration

Look at [Excision Mail](https://github.com/Excision-Mail/Excision-Mail) for a complex playbook example.
