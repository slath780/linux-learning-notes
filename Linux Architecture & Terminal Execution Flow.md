

What is Linux Architecture?

Linux is organized into layers. Each layer has a specific role and communicates with the layer below it.

User  
 ↓  
Shell  
 ↓  
Kernel  
 ↓  
Hardware
### User
The user is the person interacting with the system.

Examples:
- Running commands
- Opening applications
- Managing files

The user does not communicate directly with the hardware.

### Shell
The Shell is the interface between the user and the operating system.

Responsibilities:
- Receives commands
- Interprets commands
- Finds programs
- Sends requests to the Kernel

Examples:
- bash
- zsh
- fish 

### Kernel
The Kernel is the core of the operating system.

Responsibilities:
- CPU management
- Memory management
- Process management
- File system management
- Network management
- Hardware communication

Programs do not access hardware directly. They request services from the Kernel.

### User Space vs Kernel Space

#### User Space
Contains normal applications such as:
- Firefox
- Chrome
- VSCode
- Terminal
- Python

Applications in User Space cannot directly access hardware.

#### Kernel Space
Contains the Kernel.

The Kernel has full access to:
- CPU
- RAM
- Disk
- Network devices
- Hardware components

### Command Execution Flow

Example:
`date`

Execution flow:
1. User types a command.
2. Shell receives the command.
3. Shell locates the program.
4. Shell asks the Kernel to execute it.
5. Kernel runs the process.
6. Output is returned to the Terminal.

User  
 ↓  
Shell  
 ↓  
Kernel  
 ↓  
Hardware
↓
Result 
### What is a Process?
A Process is a program currently running in memory.

Examples:
- Chrome
- Firefox
- VSCode
- Bash

Each process has a unique identifier called:
- PID 

### Process Management Commands

Show running processes:
ps 

Show detailed processes:
ps aux 

Display current user:
whoami 

Display user information:
id 

### User vs Root

#### User
Regular account with limited permissions.

Can:
- Create files
- Run applications
- Access personal data

Cannot:
- Modify critical system files
- Perform administrative actions

#### Root
The superuser account.

Can:
- Access any file
- Modify system settings
- Manage users
- Control services

Root has unrestricted access to the system.

### Why is Root Important?
Linux follows the principle of:
- Least Privilege 

Users and programs should only have the permissions they actually need. This improves security and system stability.

### Summary
Linux uses a layered architecture:

User  
 ↓  
Shell  
 ↓  
Kernel  
 ↓  
Hardware

The Kernel acts as the central manager of the operating system, controlling resources, processes, permissions, and communication with hardware.
