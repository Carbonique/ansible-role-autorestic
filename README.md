- [About](#about)
- [Defaults & Variables](#defaults--variables)

# About

This role installs [Restic](https://github.com/restic/restic) and [Autorestic](https://github.com/cupcakearmy/autorestic/) and setups a generates an `autorestic.yml` config file.
As backup backend it uses a B2 bucket and local storage. At this moment, only these 2 backup locations are supported
The role also assumes the user has existing Autorestic backup keys. 

Credits go to [Agate](https://code.agate.blue/agate/autorestic-backup-ansible-role)

# Defaults & Variables

Defaults have been prefilled, variables have to be filled by the user.
