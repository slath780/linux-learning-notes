# Linux Permissions

## Permission Types

r = read
w = write
x = execute

---

# Permission Groups

Permissions are divided into:
- Owner
- Group
- Others

Example:
rw-r--r--

---

# chmod

Used to change permissions.

Examples:
chmod +x script.sh
chmod 755 script.sh

---

# chown

Changes file owner.

Example:
sudo chown trainee file.txt

---

# chgrp

Changes file group.

Example:
sudo chgrp analyst file.txt

---

# Important Concepts

## SUID
Allows a file to run with owner privileges.

Find SUID files:
find / -perm -4000 2>/dev/null

---

## Sticky Bit

Commonly used on:
/tmp

Prevents users from deleting other users' files.