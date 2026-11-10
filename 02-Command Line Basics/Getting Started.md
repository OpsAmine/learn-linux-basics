# Getting Started with Terminal 

## What is a Command?

A **command** is a program that instructs the operating system to perform a specific task. In Linux, programs are stored as files on the filesystem. Therefore, commands are executable files located in specific directories on the disk.

Commands can also accept additional inputs called **command-line arguments**, which allow users to specify how a command should behave or what task it should perform.

Understanding how to use commands is essential when working with Linux. Fortunately, Linux provides several built-in ways to get help and learn more about commands, their options, and their usage.


## What is a Terminal?

The **terminal** is a text-based interface that lets you control your computer by typing commands instead of clicking with a mouse

### Core Layers
To understand what the terminal actually does, it helps to see how it fits alongside other parts of the system:

- **The Terminal (or terminal Emulator):**  The window application that displays the text and handles your keyboard and screen input. It does not actually understand the commands you type; it just passes them along.

- **The Shell:**  The program running inside the terminal that actually reads your text, interprets what you mean, and tells the system what to do.

- **The Kernel:** The core of the Linux operating system that manages your hardware (CPU, memory, storage).

## What Can You Do in the Terminal?
• **File Management:** Create, copy, move, or delete files and folders.
• **System Administration:** Install or update software, check running processes, or change user permissions.
• **Automation:** Write scripts to run repetitive tasks automatically.
• **Remote Control:** Log into and manage remote servers that do not have a graphical desktop interface.


## Linux FileSystem
The **Linux filesystem** follows a hierarchical (tree-like) structure, starting from the top-level directory known as the **root directory**, represented by `/`. All files and directories in a Linux system originate from this directory. Its subdirectories organize files based on their purpose, including system configurations, application files, user data, and other resources. Each directory can contain additional files and subdirectories, forming a structured hierarchy.

```bash
/
├── bin/
├── boot/
├── dev/
├── etc/
├── home/
│   ├── user1/
│   └── user2/
├── lib/
├── media/
├── mnt/
├── opt/
├── proc/
├── root/
├── run/
├── sbin/
├── srv/
├── sys/
├── tmp/
├── usr/
│   ├── bin/
│   ├── lib/
│   └── sbin/
└── var/
    ├── lib/
    └── log/
```
| **Directory** | **Description** |
| :------------ | :-------------- |
| `/`           | The root directory, which is the starting point of the entire Linux filesystem hierarchy. |
| `/bin`        | Contains essential command-line executables required by users and the system. |
| `/boot`       | Contains files required to boot the system, including the Linux kernel and bootloader files. |
| `/dev`        | Contains device files that provide access to hardware and virtual devices. |
| `/etc`        | Contains system-wide configuration files and settings. |
| `/home`       | Contains personal directories and files belonging to regular users. |
| `/lib`        | Contains essential shared libraries and kernel modules required by system programs. |
| `/media`      | Provides mount points for removable media, such as USB drives and optical discs. |
| `/mnt`        | Used as a temporary mount point for filesystems and storage devices. |
| `/opt`        | Contains optional application software and third-party packages. |
| `/proc`       | A virtual filesystem that provides information about running processes and kernel parameters. |
| `/root`       | Contains the personal files and configuration settings of the root user. |
| `/run`        | Stores temporary runtime data about running processes and system services. |
| `/sbin`       | Contains essential system administration executables. |
| `/srv`        | Contains data served by system services, such as web or FTP servers. |
| `/sys`        | A virtual filesystem that exposes information about devices, drivers, and the kernel. |
| `/tmp`        | Stores temporary files that applications and users may create during system operation. |
| `/usr`        | Contains user-space applications, utilities, libraries, and shared resources. |
| `/var`        | Contains variable data such as logs, caches, databases, and application state files. |

On modern Linux distributions, **/bin**, **/sbin**, and **/lib** are often symbolic links to their corresponding directories under **/usr**
