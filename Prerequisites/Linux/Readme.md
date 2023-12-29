# Introduction

Linux is an operating system, with its core being a kernel that interacts with hardware, making it function and enabling program execution.

## Why Command-Line Interface?

The command-line interface is essential for effective work on your Linux laptop, providing greater functionality compared to the limitations of a graphical user interface (GUI).

## Basic Linux Commands

- `whoami`: Check current user
- `touch file_name.txt`: Create a file
- `pwd`: Check current working directory
- `mkdir foldername`: Create a directory (folder)
- `ls`: List contents in the current directory
- `cd dirname`: Change directory
- `cd ..`: Move one directory back
- `mv src_path destination_path`: Move a file or directory
- `cat filename`: View contents of a file
- `clear`: Clear the terminal
- `echo "your text"`: Print something
- `ls -la`: List contents of a directory with file info
- `nano filename`: Write something to a file using the Nano text editor
  - To exit Nano: `Ctrl + X`, press `Y` for yes to save or `N` for no, then press `Enter`
- `history`: View all previously executed commands
- `rm filename`: Delete a file (be cautious before deleting)
- `man command_name`: Access the manual for a specific command
- `sudo apt-get update`: Update package lists
- `sudo apt-get install package_name`: Install a package

## Understanding Paths in File Systems

A path represents the unique location of a file or folder within an OS file system. It comprises forward slashes (/) & alphanumeric characters.

### Absolute Path

An absolute path defines the precise location of a file or directory from the root directory (/) of the file system. In simpler terms, it represents a complete path starting from the root of the actual file system.

#### Examples of Absolute Path:
- `/home/user/documents/file.txt`
- `/var/www/html/index.html`

All these paths begin with the root directory (/), which serves as the starting point for every Linux/Unix system.

### Relative Path

A relative path is a path related to the present working directory (PWD). It indicates the location of a file or directory in relation to the present working directory (PWD) without providing the complete absolute path starting from the root directory.

#### Examples of Relative Path:
- `../parent_directory/file.txt`
- `subdirectory/image.jpg`

A relative path is like giving directions from your current location on a map, rather than starting from the very beginning.

## DevOps Overview

### What is DevOps?

DevOps is a collaborative approach to software development that bridges the gap between development (Dev) and operations (Ops) teams. It's not just a set of tools, but a philosophy that prioritizes:

- Developers and operations work together throughout the entire software lifecycle, from planning and coding to deployment and monitoring.
- Repetitive tasks are automated, freeing up time for strategic improvements.
- Changes are delivered frequently, and feedback is gathered as early as possible to ensure quality and value.

### Why do we need DevOps?

In today's fast-paced world, traditional software development processes are too slow and prone to errors. DevOps enables organizations to:

- Deliver software faster and more frequently, adapting to changing market demands.
- Improve software quality and reliability by catching bugs early in the development cycle.
- Reduce costs by streamlining the development and deployment process.
- Increase team morale and productivity by creating a more collaborative and rewarding work environment.

### DevOps Collaboration and Benefits

DevOps enables coordination and collaboration between formerly siloed roles like development, IT operations, quality engineering, and security.

Teams adopt DevOps culture, practices, and tools to increase confidence in the applications they build, respond better to customer needs, and achieve business goals faster. DevOps helps teams continually provide value to customers by producing better, more reliable products.

For more detailed information, you can explore Microsoft's DevOps documentation on [What is DevOps?](https://learn.microsoft.com/en-us/devops/what-is-devops)

### Introduction To Shell