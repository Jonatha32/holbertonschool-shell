# Shell Init Files, Variables, and Expansions

This directory contains a collection of Bash scripts that demonstrate shell initialization files, variable management, and various types of expansions in Unix-like operating systems. Each script performs a specific task related to shell environment configuration and manipulation.

## Scripts Description

| Script | Description |
|--------|-------------|
| `0-alias` | Creates an alias named `ls` with the value `rm *` using the `alias` command. |
| `1-hello_you` | Prints "hello user", where user is the current Linux user, using the `$USER` environment variable. |
| `2-path` | Adds `/action` to the `PATH` environment variable, making it the last directory the shell looks into when looking for a program. |
| `3-paths` | Counts the number of directories in the `PATH` environment variable using parameter expansion and the `tr` command. |
| `4-global_variables` | Lists all environment variables using the `printenv` command. |
| `5-local_variables` | Lists all local variables and environment variables, and functions using the `set` command. |
| `6-create_local_variable` | Creates a new local variable named `BEST` with the value `School`. |
| `7-create_global_variable` | Creates a new global variable named `BEST` with the value `School` using the `export` command. |
| `8-true_knowledge` | Prints the result of the addition of 128 with the value stored in the environment variable `TRUEKNOWLEDGE` using arithmetic expansion. |
| `9-divide_and_rule` | Prints the result of `POWER` divided by `DIVIDE` environment variables using arithmetic expansion. |
| `10-love_exponent_breath` | Displays the result of `BREATH` to the power of `LOVE` environment variables using arithmetic expansion. |
| `11-binary_to_decimal` | Converts a number from base 2 (stored in the environment variable `BINARY`) to base 10 using arithmetic expansion. |
| `12-combinations` | Prints all possible combinations of two lowercase letters, except `oo`, using brace expansion and filtering. |
| `13-print_float` | Prints a number (stored in the environment variable `NUM`) with two decimal places using the `printf` command. |
| `14-decimal_to_hexadecimal` | Converts a number from base 10 (stored in the environment variable `DECIMAL`) to base 16 using arithmetic expansion. |
| `15-rot13` | Encodes and decodes text using the rot13 encryption using the `tr` command. |

## Concepts Covered

- Shell initialization files (`/etc/profile`, `/etc/profile.d`, `~/.bash_profile`, `~/.bashrc`, etc.)
- Variables (local and environment)
- Variable expansions and substitutions
- Shell arithmetic
- The `alias` command
- Technical writing and documentation

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

- What are the `/etc/profile` file and the `/etc/profile.d` directory
- What is the `~/.bashrc` file
- The difference between a local and a global variable
- What is a reserved variable
- How to create, update and delete shell variables
- What are the special parameters `$?`, `$$`, `$#`, etc.
- What is expansion and how to use them
- What is the difference between single and double quotes
- How to perform command substitution
- How to perform arithmetic operations in the shell
- How to create and use aliases