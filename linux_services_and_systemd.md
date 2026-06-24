# Linux Services and systemd

What is a Service?

A service is a program that runs in the background and provides a continuous function to the system or users.

### Examples:
- SSH Server
- NetworkManager
- Bluetooth Service
- Cron Scheduler

Unlike normal programs, services are usually started automatically and continue running without user interaction.

---

# What is systemd?

systemd is the system and service manager used by most modern Linux distributions.

It is usually the first userspace process started after the kernel and commonly has PID 1.

Main responsibilities:
- Start services during boot
- Stop services
- Restart services
- Monitor service status
- Enable or disable services at startup

---

# Service vs Process

A process is a running instance of a program.
A service is a managed background function that may run one or more processes.

Example:
SSH Service
    ↓
sshd Process

The service provides the function, while the process performs the actual work.

---

# Linux Control Flow

User
 ↓
Shell
 ↓
systemd
 ↓
Service
 ↓
Process

### User
The person who requests an action from the system.

### Shell
Receives commands from the user, interprets them, and requests execution.

### systemd
Manages services and system behavior.

### Service
Provides a continuous function in the background.

### Process
Performs the actual execution of work.

---

Common systemctl Commands

Check service status:
systemctl status service_name

Start a service:
systemctl start service_name

Stop a service:
systemctl stop service_name

Restart a service:
systemctl restart service_name

Enable a service at boot:
systemctl enable service_name

Disable a service at boot:
systemctl disable service_name

---

# Summary

A service is a background program that provides a continuous function.
A process is a running instance of a program.
systemd manages services and system startup.
Most modern Linux systems use systemd as PID 1.
Services are controlled using the systemctl command.
