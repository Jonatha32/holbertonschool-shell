# Shell Permissions

This directory contains a collection of Bash scripts that demonstrate various aspects of file permissions, ownership, and access control in Unix-like operating systems. Each script performs a specific task related to managing permissions.

## Scripts Description

| Script | Description |
|--------|-------------|
| `0-iam_betty` | Switches the current user to the user `betty` using the `su` command. |
| `1-who_am_i` | Prints the effective username of the current user using the `id -un` command. |
| `2-groups` | Prints all the groups the current user is part of using the `groups` command. |
| `3-new_owner` | Changes the owner of the file `hello` to the user `betty` using the `chown` command. |
| `4-empty` | Creates an empty file called `hello` using the `touch` command. |
| `5-execute` | Adds execute permission to the owner of the file `hello` using the `chmod u+x` command. |
| `6-multiple_permissions` | Adds execute permission to the owner and the group owner, and read permission to other users, to the file `hello` using the `chmod 754` command. |
| `7-everybody` | Adds execution permission to the owner, the group owner and all other users, to the file `hello` using the `chmod a+x` command. |
| `8-James_Bond` | Sets the permission to the file `hello` as follows: Owner: no permission at all, Group: no permission at all, Other users: all the permissions (007) using the `chmod 007` command. |
| `9-John_Doe` | Sets the mode of the file `hello` to `-rwxr-x-wx` (753) using the `chmod 753` command. |
| `10-mirror_permissions` | Sets the mode of the file `hello` the same as `olleh`'s mode using the `chmod --reference=olleh hello` command. |
| `11-directories_permissions` | Adds execute permission to all subdirectories of the current directory for the owner, the group owner and all other users using the `chmod -R +X .` command. |
| `12-directory_permissions` | Creates a directory called `my_dir` with permissions 751 in the working directory using the `mkdir -m 751` command. |
| `13-change_group` | Changes the group owner to `school` for the file `hello` using the `chgrp` command. |
| `14-change_owner_and_group` | Changes the owner to `vincent` and the group owner to `staff` for all the files and directories in the working directory using the `chown -hR` command. |
| `15-symbolic_link_permissions` | Changes the owner and the group owner of the symbolic link `_hello` to `vincent` and `staff` respectively using the `chown -h` command. |
| `16-if_only` | Changes the owner of the file `hello` to `vincent` only if it is owned by the user `guillaume` using the `chown --from=` option. |

## Concepts Covered

- User and group ownership in Unix-like systems
- File and directory permissions
- Symbolic and numeric permission notation
- Special permission bits
- Changing ownership and permissions
- Recursive permission changes
- Reference-based permission setting
- Conditional ownership changes

## Usage

All scripts are executable and can be run directly from the command line:

```bash
./script-name
```

Make sure all scripts have execution permissions:

```bash
chmod +x script-name
```

## Requirements

- All scripts are interpreted on Ubuntu 20.04 LTS
- All scripts are exactly two lines long (including the shebang line)
- All files end with a new line
- The first line of all files is `#!/bin/bash`
- No use of backticks, &&, ||, or ;
- All commands have exactly the required number of flags/options

## Learning Objectives

Through these scripts, you will learn:

- What do the commands `chmod`, `sudo`, `su`, `chown`, `chgrp` do
- Linux file permissions
- How to represent each of the three sets of permissions (owner, group, and other) as a single digit
- How to change permissions, owner and group of a file
- Why can't a normal user `chown` a file
- How to run commands with root privileges
- How to change user ID or become superuser