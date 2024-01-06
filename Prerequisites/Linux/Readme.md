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

Commands in Linux can be generally categorized into two types:
- Internal or Built-in commands :
  Internal commands are part of the shell itself and come bundled with it. Common built-in commands include echo, cd, pwd, mkdir, etc.
- External Commands :
  External commands are binary programs or scripts which are usually located in distinct files in the system. They either come pre-installed with distribution's package manager or can be created or installed by the user.
  Examples:
  mv, date, uptime, cp, etc.
  Also, use the "type" command to determine if a command is internal or external. For example, the echo command is a shell built-in, and the mv command is an external command.
  
## Using command line to get help

In this section we will learn how to use **`help`** command to get help in command line
- If you are new to using linux or bash shell or if you are not sure which command does what, there are few commands in bash that can help get started. 
- Lets take a look of those

First command is **`whatis`** , this command will displays a one line description of a command does. 

**`Syntax: whatis <command>`**

```
$ whatis date
```

Most of the commands internal or external come bundled with **`man pages`** which provides information about the command in detail (with examples, usecases and with command options)

**`Syntax: man <command>`**

```
$ man date
```

Several commands will provide **`-h`** or **`--help`** to provide users with the options and usecases available in a command

```
$ date -h
$ date --help
```

To search through the man page names and descriptions for instances of the keyword use **`apropos`**. This is useful if you want to look for all commands within the system that contains the specifc keyword.

**`Syntax: apropos <keyword>`**
```
$ apropos modpr
```  
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

## Fundamentals of DevOps

### Chapters:

1. **Version Control System (VCS)**
   
2. **Continuous Integration and Continuous Deployment (CI/CD)**
   
3. **Infrastructure as Code (IaC)**
   
4. **Configuration Management**
   
5. **Containerization**
   
6. **Monitoring/Observability**

## Linux and Docker Fundamentals

[Session Link](https://www.youtube.com/live/EUu1E_YKGTw?feature=shared)

## Linux File System 

### Introduction to File System Structure

Linux organizes its file system in a hierarchical structure, starting from the root directory ("/"). Each directory in the system has its own purpose and contains various files and subdirectories.

### Key Directories in Linux File System

#### /

The root directory contains all other directories and files. It is represented by `/`.

#### /home

Contains home directories and files for users.

#### /bin

Holds user command binaries such as `cat`, `echo`, etc.

#### /sbin

Stores system binaries, requiring sudo privileges to access.

#### /usr

Contains user-related data and executables.

#### /usr/bin 
Primary executables that the system needs in order to run.

#### /usr/local 
Programs installed just for that user.

#### /lib 
When executables in /bin need additional library files in order to run.

#### /var 
Variable data (temporary).

#### /var/log 
Logs are stored here usually for 30 days.

#### /var/log/syslog 
System logs.

#### /var/cache 
Cached data from programs.

#### /opt 
Programs that install everything in one directory (not separated in /bin and /lib).

#### /etc 
System-wide configurations.

#### /etc/fstab 
Controls how different filesystems are treated each time they are introduced to a system.

#### /etc/hosts 
Used to translate hostnames to IP-addresses.

#### /etc/hostname 
Name of the machine.

#### /etc/sudoers 
Specifies who can act as the superuser (sudo).

#### /tmp 
Temporary location for running processes.

#### /boot 
Do not touch - for booting the system.

#### /dev 
Devices configurations like mouse and keyboard.

#### /media 
Devices like CD or USB drive auto-mounts here.

#### /mnt 
Temporary mount points for additional filesystems.

#### CHALLENGE 1
- Using commands inside the terminal, Find out what operating system you are running
- Find where the system log (syslog) is in Linux. View the file once found.
- create new user named "chris" with bash as default shell
- create new group named "docker" and add "chris" to it

```
cd /
pwd
ls

# find the release info
lsb_release -a
cat /etc/os-release
uname -a
lscpu
lsmem

# find syslog
find / -name 'syslog'
find / -iname 'syslog'

# change directory to where syslog is
cd /var/log/

# view the syslog
cat /var/log/syslog
cat /var/log/syslog | less
```