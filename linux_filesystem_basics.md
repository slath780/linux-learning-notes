# Linux Filesystem Basics

## Root Directory

The root directory is:

/

All files and directories in Linux start from the root directory.

---

# Important Directories

## /home

Stores user home directories.

Example:
/home/salah

Contains:
- Documents
- Scripts
- Downloads
- Personal files

---

## /etc

Contains system configuration files.

Examples:
- /etc/passwd
- /etc/shadow
- /etc/hosts

---

## /var

Stores variable data.

Important subdirectories:
- /var/log
- /var/cache

Used for:
- Logs
- Services
- Runtime data

---

## /tmp

Temporary storage directory.

Commonly used by:
- Applications
- Scripts
- System processes

---

## /dev

Represents hardware devices as files.

Examples:
- /dev/sda
- /dev/null
- /dev/random

---

## /proc

Virtual filesystem created by the kernel.

Contains:
- Process information
- CPU information
- Memory information

Useful commands:
cat /proc/cpuinfo
cat /proc/meminfo

---

## /bin

Contains essential executable binaries.

Examples:
- ls
- cp
- mv
- cat

---

## /usr

Contains user applications, libraries, and utilities.

Important directory:
/usr/bin

---

## /sys

Virtual filesystem for hardware and kernel devices.

Contains:
- Network interfaces
- Drivers
- Kernel device information

---

# Important Concept

In Linux, almost everything is treated as a file:
- Devices
- Processes
- Terminals
- Hardware interfaces
