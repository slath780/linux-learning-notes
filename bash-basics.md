# Bash Basics

## What is Bash?

Bash is a shell.

It allows users to interact with Linux using commands.

---

## What is a Shell?

The shell acts as a bridge between the user and the operating system.

User -> Shell -> Kernel

---

## Bash Script

A Bash script is a file containing multiple Bash commands.

Example:

#!/bin/bash

echo "Hello"

---

## Shebang

#!/bin/bash

Tells Linux to execute the file using Bash.

---

## Variables

Example:

name="Salah"

echo $name

---

## User Input

Example:

read name

echo $name

---

## Conditions

Example:

if [ $age -ge 18 ]
then
    echo "Adult"
fi

---

## Loops

Example:

for i in 1 2 3
do
    echo $i
done