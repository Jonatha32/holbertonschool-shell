# Shell I/O Redirections and Filters

This directory contains a collection of Bash scripts that demonstrate input/output redirections and text processing filters in Unix-like operating systems. Each script performs a specific task related to file content manipulation, text processing, and data filtering.

## Scripts Description

| Script | Description |
|--------|-------------|
| `0-hello_world` | Prints "Hello, World" followed by a new line to the standard output using the `echo` command. |
| `1-confused_smiley` | Displays a confused smiley `"(Ôo)'` using proper escaping techniques. |
| `2-hellofile` | Displays the content of the `/etc/passwd` file using the `cat` command. |
| `3-twofiles` | Displays the content of `/etc/passwd` and `/etc/hosts` files using the `cat` command with multiple arguments. |
| `4-lastlines` | Displays the last 10 lines of `/etc/passwd` using the `tail` command. |
| `5-firstlines` | Displays the first 10 lines of `/etc/passwd` using the `head` command. |
| `6-third_line` | Displays the third line of the file `iacta` using a combination of `head` and `tail` commands. |
| `7-file` | Creates a file named `\*\\'"Best School"\'\\*$\?\*\*\*\*\*:)` containing the text "Best School" using proper escaping techniques. |
| `8-cwd_state` | Writes the result of the command `ls -la` into the file `ls_cwd_content` using output redirection. |
| `9-duplicate_last_line` | Duplicates the last line of the file `iacta` using a combination of `tail` and redirection operators. |
| `10-no_more_js` | Deletes all regular files with a `.js` extension in the current directory and all its subfolders using the `find` command. |
| `11-directories` | Counts the number of directories and sub-directories in the current directory using the `find` command with appropriate options. |
| `12-newest_files` | Displays the 10 newest files in the current directory, sorted from newest to oldest using a combination of `ls` and `sort` commands. |
| `13-unique` | Takes a list of words as input and prints only words that appear exactly once using the `sort` and `uniq` commands. |
| `14-findthatword` | Displays lines containing the pattern "root" from the file `/etc/passwd` using the `grep` command. |
| `15-countthatword` | Displays the number of lines that contain the pattern "bin" in the file `/etc/passwd` using the `grep` command with the `-c` option. |
| `16-whatsnext` | Displays lines containing the pattern "root" and 3 lines after them in the file `/etc/passwd` using the `grep` command with the `-A` option. |
| `17-hidethisword` | Displays all the lines in the file `/etc/passwd` that do not contain the pattern "bin" using the `grep` command with the `-v` option. |
| `18-letteronly` | Displays all lines of the file `/etc/ssh/sshd_config` starting with a letter using the `grep` command with a regular expression. |
| `19-AZ` | Replaces all characters `A` and `c` from input to `Z` and `e` respectively using the `tr` command. |
| `20-hiago` | Removes all letters `c` and `C` from input using the `tr` command with the `-d` option. |
| `21-reverse` | Reverses its input using the `rev` command. |
| `22-users_and_homes` | Displays all users and their home directories, sorted by users, based on the `/etc/passwd` file using a combination of `cut`, `sort`, and other commands. |

## Concepts Covered

- Standard input, output, and error streams
- Input/output redirection operators (>, >>, <, <<, |)
- Text processing tools (cat, head, tail, find, grep, tr, sort, uniq, cut)
- Regular expressions
- File content manipulation
- Command pipelines
- Filtering and transforming text

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

- How to redirect standard input, output, and error
- How to use pipelines to connect commands together
- How to filter and process text using various command-line tools
- How to use regular expressions for pattern matching
- How to combine multiple commands to solve complex text processing tasks