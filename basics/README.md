# Shell Basics

This directory contains a collection of Bash scripts that demonstrate fundamental shell commands and operations in Unix-like operating systems. Each script performs a specific task related to file navigation, manipulation, and basic shell operations.

## Scripts Description

| Script | Description |
|--------|-------------|
| `0-current_working_directory` | Prints the absolute path of the current working directory using the `pwd` command. |
| `1-listit` | Displays the contents of the current directory using the `ls` command. |
| `2-bring_me_home` | Changes the working directory to the user's home directory using the `cd` command without arguments. |
| `3-listfiles` | Displays current directory contents in a long format using the `ls -l` command. |
| `4-listmorefiles` | Displays current directory contents, including hidden files, in long format using the `ls -la` command. |
| `5-listfilesdigitonly` | Displays current directory contents in long format with user and group IDs displayed numerically, including hidden files, using the `ls -na` command. |
| `6-firstdirectory` | Creates a directory named `my_first_directory` in the `/tmp/` directory using the `mkdir` command. |
| `7-movethatfile` | Moves the file `betty` from `/tmp/` to `/tmp/my_first_directory/` using the `mv` command. |
| `8-firstdelete` | Deletes the file `betty` from `/tmp/my_first_directory/` using the `rm` command. |
| `9-firstdirdeletion` | Deletes the directory `my_first_directory` that is in the `/tmp` directory using the `rmdir` command. |
| `10-back` | Changes the working directory to the previous one using the `cd -` command. |
| `11-lists` | Lists all files in the current directory, parent directory, and `/boot` directory in long format using the `ls -la` command with multiple arguments. |
| `12-file_type` | Prints the type of the file named `iamafile` in the `/tmp` directory using the `file` command. |
| `13-symbolic_link` | Creates a symbolic link to `/bin/ls`, named `__ls__` in the current directory using the `ln -s` command. |
| `14-copy_html` | Copies all HTML files from the current working directory to the parent directory, but only copies files that did not exist in the parent directory or were newer than the versions in the parent directory using the `cp -u` command. |
| `15-lets_move` | Moves all files beginning with an uppercase letter to the directory `/tmp/u` using the `mv` command with pattern matching. |
| `16-clean_emacs` | Deletes all files in the current working directory that end with the character `~` using the `rm` command with pattern matching. |
| `17-tree` | Creates the directories `welcome/`, `welcome/to/` and `welcome/to/school` in the current directory using the `mkdir -p` command. |

## Concepts Covered

- Navigation in the file system
- File and directory manipulation
- Working with hidden files
- Basic file operations (create, move, delete)
- Symbolic links
- Pattern matching and wildcards
- Directory structure creation

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

- What is the shell and how to navigate the filesystem
- What are the basic shell commands and how to use them
- How to manipulate files and directories
- How to work with command history and help commands
- How to use wildcards and pattern matching
- How to create and use symbolic links
- How to organize files and directories efficiently