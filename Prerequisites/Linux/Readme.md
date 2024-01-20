## Introduction

Linux is an operating system, with its core being a kernel that interacts with hardware, making it function and enabling program execution.

### Why Command-Line Interface?

The command-line interface is essential for effective work on your Linux laptop, providing greater functionality compared to the limitations of a graphical user interface (GUI).

### Basic Linux Commands

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
  
### Using command line to get help

In this section we will learn how to use **`help`** command to get help in command line
- If you are new to using linux or bash shell or if you are not sure which command does what, there are few commands in bash that can help get started. Lets take a look of those

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
### Understanding Paths in File Systems

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

### DevOps Overview

### What is DevOps?

DevOps is a collaborative approach to software development that bridges the gap between development (Dev) and operations (Ops) teams. DevOps is basically a practice or culture that improves the organizational's ability to deliver the applications. In simple words, DevOps is a process of improving the application delivery by ensuring that there is a proper automation in place with the application quality that is maintained and ensuring there is a continuous monitoring and continous testing in place. This is DevOps!

It's not just a set of tools, but a philosophy that prioritizes: 

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

### Software Development Lifecycle 

### What is SDLC ?
 
It's a step-by-step process that is followed by the industry to design, build, test and deploy software. Imagine it as a series of phases, starting with planning and ending with the release of the finished product. Each phase has its own tasks and objectives, making sure the software is developed smoothly and meets the needs of its users. 

The end goal is to deliver a high quality product. DevOps Engineers primarily focus on automating building, testing, and deployment phases to enhance software delivery efficiency. Their tasks include writing automation scripts to improve efficiency and reduce manual intervention.

Building involves writing code and storing it in repositories like Git, followed by testing on servers and deploying the application for customer access.
DevOps significantly improves efficiency and automation throughout the SDLC stages.
Collaboration is vital, especially within agile methodologies and DevOps impact is felt in both cloud-based and on-premises setups.

### What is a Server ?

A server is a computer or system that is dedicated to managing network resources and providing services to other computers, known as clients, in the network. 

Servers are designed to handle specific tasks such as hosting websites, managing databases, file storage, and more. They operate continuously and are optimized for performance, reliability and security.

### What is Virtualization ?

Virtualization is a technology that allows a single physical computer to run multiple virtual computers, each with its own operating system and applications. Instead of relying on separate physical machines for different tasks, virtualization enables the creation of virtual machines (VMs) on a single hardware platform.

### What is Virtual Machine ?

A Virtual Machine (VM) is a software-based emulation of a physical computer that runs an operating system and applications. VMs are created using virtualization technology, allowing multiple VMs to run on a single physical server. Each VM operates independently, with its own virtualized hardware resources, providing isolation and flexibility.

### What is Hypervisor ? 

A hypervisor is a software that you can use to run multiple virtual machines on a single physical machine. Every virtual machine has its own operating system and applications. The hypervisor allocates the underlying physical computing resources such as CPU and memory to individual virtual machines as required.

### Difference between Physical and Virtual Machines

### Physical Machines

- Exist as tangible hardware components.
- Run a single operating system directly on the physical hardware.
- Limited scalability, as each machine requires dedicated physical resources.
- Resource utilization may not be optimal, leading to inefficiencies.

### Virtual Machines

- Exist as software-based emulations on a physical server.
- Run multiple operating systems simultaneously on the same physical hardware.
- Enhanced scalability, as multiple VMs can share the same physical resources.
- Improved resource utilization, allowing for more efficient use of hardware resources.

### Advantages of Virtual Machines :

- It efficiently shares and allocates resources among multiple VMs on a single physical server.

- VMs operate independently, providing isolation between applications and operating systems.

- VMs can be easily moved or replicated across different physical servers, offering flexibility and portability.

- It dynamically allocates resources to VMs, allowing for flexible scaling based on workload demands.

- Reduces hardware costs and energy consumption through the consolidation of multiple VMs on a single server.

- VMs provides a controlled environment for testing and development without impacting production systems.

### What is EC2 Instance ?

An EC2 instance is a virtual server within Amazon Web Services (AWS) Elastic Compute Cloud (EC2), enabling users to run applications on the AWS infrastructure. 

These instances offer flexibility, scalability and a variety of configurations to cater to diverse workloads and performance requirements.

### Key Characteristics :

- EC2 instances are virtual machines (VMs) running on physical servers in AWS data centers.

- Users can easily scale compute capacity up or down, making EC2 suitable for dynamic workloads.

- AWS provides multiple instance types optimized for different use cases, including compute-optimized, memory-optimized, storage-optimized, and GPU instances.

- Users can customize EC2 instances with various options such as operating systems, storage volumes, network settings, and security configurations.

- EC2 follows a pay-as-you-go pricing model, allowing users to pay for the compute capacity they consume.

### Significance in AWS

EC2 instances form the backbone of AWS's cloud computing services, serving as the fundamental infrastructure for deploying and running applications in the cloud.

### What is Cloud Computing ?

Cloud computing is the on-demand delivery of IT resources over the Internet with pay-as-you-go pricing. Instead of buying, owning, and maintaining physical data centers and servers, you can access technology services, such as computing power, storage, and databases, on an as-needed basis from a cloud provider like Amazon Web Services (AWS).

### Fundamentals of DevOps

### Chapters:

1. **Version Control System (VCS)**
   
2. **Continuous Integration and Continuous Deployment (CI/CD)**
   
3. **Infrastructure as Code (IaC)**
   
4. **Configuration Management**
   
5. **Containerization**
   
6. **Monitoring/Observability**

### Linux and Docker Fundamentals

[Session Link](https://www.youtube.com/live/EUu1E_YKGTw?feature=shared)

### Linux File System 

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
- create new user named "tejas" with bash as default shell
- create new group named "docker" and add "tejas" to it

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

# View default options for new users
# The 'man' command displays the manual for 'useradd'
man useradd
# 'useradd -D' displays the default options used by 'useradd'

# Change the default shell for new users from Bourne shell to Bourne Again SHell (bash)
useradd -D -s /bin/bash

# Check which shell you're currently using
echo $0   # Displays the currently running shell for the current session
echo $SHELL  # Displays the default shell for the user

# Display all available shells on the system
cat /etc/shells   # Lists all available shells configured on the system

# Create a new user 'tejas' with a home directory
useradd -m tejas   # '-m' creates the home directory for the user

# Set a password for the newly created user 'tejas'
passwd tejas   # Prompts to set a password for the 'tejas' user

# Grant sudo privileges to the 'tejas' user
usermod -aG sudo tejas   # Adds 'tejas' to the sudo group

# Switch to the 'tejas' user
su - tejas   # Switches the current session to the 'tejas' user with their environment

# add group
To add a new group named "docker", use the following command:
groupadd docker

# get group info
getent group docker

# add your user to the docker group
sudo usermod -aG docker $USER

# what groups user is in
groups tejas
cat /etc/group
```