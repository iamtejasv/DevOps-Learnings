## Introduction

### What is Terminal ?

A **terminal** is a text-based interface that allows users to interact with their computer using commands. It provides a way to input text commands and receive text-based output. Terminals are powerful tools for users who prefer command-line interactions over graphical user interfaces (GUI).

### What is a Shell ?

The **shell** is a program that interprets and executes user commands. It acts as an interface between the user and the operating system. Bash (Bourne Again SHell) is a popular shell that comes pre-installed on most Unix-based systems, including Linux and macOS. It provides a set of commands and features to navigate the file system, manage processes and automate tasks.

## Terminal Navigation with Bash

These are the essential commands for navigating the terminal with Bash. Let's explore the key commands :

### pwd (Print Working Directory)

The `pwd` command prints the current working directory. It's handy for quickly checking where you are in the file system.

### cd (Change Directory)

Use the `cd` command to change to a different directory. For instance, entering `cd ~` takes you to your home directory.

### pushd and popd

- **pushd:** Adds the current directory to a stack.
- **popd:** Removes the top directory from the stack, making it the current directory. This is useful for easy navigation between directories.

### File System Navigation Notations

- Use `.` for the current directory.
- Use `..` for the parent directory.

## File and Directory Listing

### `ls` (List)

The `ls` command is used to list the contents of a directory. Adding options such as `-l` provides detailed information about files and directories.

### `tree`

The `tree` command displays the directory structure in a tree-like format, showing the hierarchy of files and subdirectories.

## File Manipulation

### `touch`

The `touch` command is used to create empty files. For example, `touch filename.txt` creates a new file named "filename.txt."

### `mkdir` (Make Directory)

Use the `mkdir` command to create a new directory. For example, `mkdir new_directory` creates a new directory named "new_directory."

### `cp` (Copy) & `mv` (Move)

- `cp` is used to copy files or directories. For example, `cp file.txt /path/to/destination` copies "file.txt" to the specified destination.
- `mv` is used to move files or directories. It can also be used for renaming. For example, `mv file.txt new_file.txt` renames "file.txt" to "new_file.txt."

### `rm` (Remove)

The `rm` command is used to delete files or directories. Be caution with this command, as it deletes files permanently. For example, `rm file.txt` deletes "file.txt."

## File Content Viewing

### `cat` and `less`

- `cat` displays the entire contents of a file. For example, `cat file.txt` shows the contents of "file.txt."
- `less` allows you to view the contents of a file one screen at a time, providing better navigation for large files.

## File Searching

### `grep`

The `grep` command is used for searching text within files. It stands for "Global Regular Expression Print". For example, `grep "keyword" file.txt` searches for the specified keyword in "file.txt". grep is powerful and can be combined with other commands and options to make your searches more flexible.

## System Information

### `uname`

The `uname` command provides system information. It stands for "Unix Name. For example, `uname -a` displays detailed information about the system.