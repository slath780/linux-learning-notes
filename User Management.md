# Linux User Management

## Linux is Multi-user
Linux is designed to support multiple users securely.

Each user has:
- Username
- UID
- GID
- Home directory
- Shell
- Permissions

---

# Important Files

## /etc/passwd
Stores user account information.

Example:
cat /etc/passwd

---

## /etc/shadow
Stores encrypted passwords.

Only root can access it.

---

## /etc/group
Stores group information.

---

# Important Concepts

## UID
User ID used internally by Linux.

## GID
Group ID used for permission management.

## Root User
UID 0.
Has full control over the system.

## sudo
Allows temporary administrative privileges.

---

# Useful Commands

## Show current user
whoami

## Show user identity
id

## Add new user
sudo adduser trainee

## Switch user
su - trainee

## Show groups
groups

## List sudo permissions
sudo -l