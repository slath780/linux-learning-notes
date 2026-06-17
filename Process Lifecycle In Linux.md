### Process Lifecycle in Linux

What is a Process?

A process is a program currently running in memory.

Examples:

- Chrome
- Firefox
- Bash
- Python

Each process has a unique identifier called PID (Process ID).

---

###  Process Lifecycle

A process goes through several states during its lifetime.

Created
↓
Ready
↓
Running
↓
Waiting / Sleeping
↓
Running
↓
Terminated

---

### 1. Created

The process is created when a program starts.

Example:

ls

The shell asks the kernel to create a new process.

---

### 2. Ready

The process is ready to run but is waiting for CPU time.

The kernel scheduler decides when it will execute.

---

### 3. Running

The process is currently executing on the CPU.

Examples:

- Reading files
- Performing calculations
- Sending network requests

---

### 4. Waiting / Sleeping

The process temporarily pauses while waiting for something.

Examples:

- Disk operations
- User input
- Network responses

After the required resource becomes available, the process returns to Running.

---

### 5. Terminated

The process finishes execution and exits.

Processes can terminate:

- Normally after completing their work.
- By receiving signals from the kernel.

---

### Process Signals

## SIGTERM (15)

Normal termination.

kill PID

The process is allowed to:

- Save data
- Close files
- Release resources

---

## SIGKILL (9)

Forced termination.

kill -9 PID

The kernel immediately stops the process.

No cleanup or saving is performed.

---

### Process Example

When running:

cat file.txt

The following occurs:

1. The shell receives the command.
2. The kernel creates a process.
3. The process waits for CPU time.
4. The process executes.
5. Output is displayed.
6. The process terminates.

---

### Summary

A process is a running instance of a program.

Typical lifecycle:

Created
↓
Ready
↓
Running
↓
Waiting
↓
Running
↓
Terminated

The Linux kernel manages all processes and controls their execution.