---
marp: true
paginate: true
color: #ffff
backgroundColor: #2A2A2A
header: '![width:100px height:100px](./img/logo.png)'
footer: "**20/10/2021 - AnthonyF**"
author: AnthonyF
---
<style>
section {
  font-family: 'Century Gothic', serif !important;
}
</style>
<!-- _class: invert -->
<!-- _header: Séance -->

# Basic GNU/Linux commands <!-- fit -->

![width:300px](./img/logo.png)

---
<!-- _class: invert -->

# Table of Contents

- Navigation in a shell
- Files and directories
- Writing and displaying

---
<!-- _class: invert -->

# FHS (**F**ilesytem **H**ierarchy **S**tandard)

FHS is a directory structure used by every Linux distros.
[More info](https://github.com/LinuxLab-ESGI/FHS-Directory-Structure)

---
<!-- _class: invert -->

# Navigation in a shell

---
<!-- _class: invert -->

# `ls`

List directory contents.
> GNU coreutils, (1) General commands
---
<!-- _class: invert -->

## Useful options with `ls`

| Arguments | Description                               |
| --------- | ----------------------------------------- |
| `-l`      | More information in list format.          |
| `-a`      | Hidden files.                             |
| `-R`      | Recursive, list files in sub-directories. |
| `-lSh`    | Sort by size with human readable.         |
| `-i`      | Inodes.                                   |
| `-n`      | Numeric UID and GID.                      |

---
<!-- _class: invert -->

# `cd`

Change the working directory.
> Built in shell command, no proper man
>`type cd`
>`help cd`
> `man builtins`

---
<!-- _class: invert -->

## Useful commands with `cd`

| Commands       | Description                               |
| -------------- | ----------------------------------------- |
| `cd ..`        | Go to parrent directory.                  |
| `cd -`         | Go back to the previous working directory |
| `cd` or `cd ~` | Go the home directory.                    |

---
<!-- _class: invert -->

# `pwd`

Print name of current working directory.
>GNU coreutils, (1) General commands

---
<!-- _class: invert -->

# Files and directories

---
<!-- _class: invert -->

# `mkdir`

Create/make directories.
Usage : `mkdir directory`
>GNU coreutiles, (1) General commands

---
<!-- _class: invert -->

## Useful options with `mkdir`

| Options | Description                                |
| ------- | ------------------------------------------ |
| `-p`    | Create parents directories if don't exist. |

---
<!-- _class: invert -->

# `rm`

Remove files or directories.
> GNU coreutils, (1) General commands

---
<!-- _class: invert -->

## Useful options with `rm`

| Options | Description                                        |
| ------- | -------------------------------------------------- |
| `-i`    | Alert before every removal.                        |
| `-d`    | Remove only empty directory.                       |
| `-r`    | Remove directories and their contents recursively. |

---
<!-- _class: invert -->

# `cp`

Copy files and directories.
Usage : `cp source destination`
> GNU coreutils, (1) General commands

---
<!-- _class: invert -->

## Useful options with `cp`

| Options | Description                   |
| ------- | ----------------------------- |
| `-d`    | No deference, preserve links. |
| `-r`    | Copy recursively.             |
| `-a`    | Same as `-dr`.                |

---
<!-- _class: invert -->

# `mv`

Move or rename files and directories.
> GNU coreutils, (1) General commands

---
<!-- _class: invert -->

# Writing and displaying

---
<!-- _class: invert -->

# `touch`

Change file timestamps.
Can also create an empty file.
> GNU coreutils, (1) General commands

---
<!-- _class: invert -->

# `cat`

Concatenate files and print on the standard output.
Can also create and write in files.
> GNU coreutils, (1) General commands

---
<!-- _class: invert -->

## Read a file

`cat file`

## Write in a file

`cat > file`

Stop writing with  `Ctrl + c`

## Add in a file

`cat >> file`

---
<!-- _class: invert -->

# Bonus "Here document"

`cat > file << EOF`

---
<!-- _class: invert -->

# `head`

Output the first part of files.
> GNU coreutils, (1) General commands

---
<!-- _class: invert -->

## Useful options with `head`

| Options   | Description                           |
| --------- | ------------------------------------- |
| `-n NUM`  | Print the first NUM lines.            |
| `-n -NUM` | Print all but not the last NUM lines. |

---
<!-- _class: invert -->

# `tail`

Output the last part of files.
> GNU coreutils, (1) General commands

---
<!-- _class: invert -->

## Useful options with `tail`

| Options   | Description                             |
| --------- | --------------------------------------- |
| `-n NUM`  | Print the last NUM lines.               |
| `-n +NUM` | Print starting at line NUM.             |
| `-f`      | Output appended data as the file grows. |


---
<!-- _class: invert -->

# Thank you ! <!-- fit-->