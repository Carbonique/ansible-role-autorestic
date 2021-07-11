- [About](#about)
- [Variables](#variables)

# About

This role installs [Restic](https://github.com/restic/restic) and [Autorestic](https://github.com/cupcakearmy/autorestic/) and setups a generates an `autorestic.yml` config file.
As backup backend it uses a B2 bucket and local HDD. At this moment, only these 2 backup locations are supported
The role also assumes the user has existing Autorestic backup keys. 

# Variables

| Variable                     | Description                                        | Default | Optional/Required |
|------------------------------+----------------------------------------------------+---------+-------------------|
| docker_encrypted_basedir     | The path for the encrypted Docker base directory   | null    | Required          |
| docker_non_encrypted_basedir | The path for the unencrypted Docker base directory | null    | Required          |
| b2_backup_bucket             | Bucket path for the Backblaze B2 backup bucket     | null    | Required          |
| b2_autorestic_key            | Autorestic key for the backup to B2                | null    | Required          |
| b2_backup_bucket_id          | Backblaze B2 bucket id                             | null    | Required          |
| b2_backup_bucket_key         | Backblaze B2 bucket key                            | null    | Required          |
| hdd_backup_path              | Path to backup to on local HDD                     | null    | Required          |
| hdd_autorestic_key           | Autorestic key for the backup to local HDD         | null    | Required          |
