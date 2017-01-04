# ansible-duply

An Ansible role for installing [Duply](http://duply.net/). In addition, this role can be used to easily backup a directory to Amazon S3.

## Role Variables

- `duply_version` - Duply version
- `duply_profile` - The name of a Duply profile
- `duply_gpg_key` - The GPG key for encrypting backups (default: `disabled`)
- `duply_gpg_pw` - The GPG password for encrypting backups
- `duply_target` - Target for your backups (see [here](http://duply.net/wiki/index.php/Duply-documentation) for details)
- `duply_target_user` - Target user
- `duply_target_pass` - Target password
- `duply_source` - Source path of backups
- `duply_max_age` - Maximum age for backups (default: `1M` for 1 month)
- `duply_max_full_age` - Maximum age of full backups
- `duply_max_full_backups` - Maximum number of full backups
- `duply_excludes` - A list of backup exclusions  (default: `[]`)

## Example Playbook

See the [examples](./examples/) directory.
