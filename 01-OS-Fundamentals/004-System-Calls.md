
# 🔄 System Calls

## How do apps interact with the Kernel?

**Answer:** Using system calls.

### Example 1: Creating a Directory

```bash
mkdir authmage
```

- `mkdir` indirectly calls the kernel and asks the file management module to create a new directory.
- `mkdir` is just a wrapper of actual system calls.
- `mkdir` interacts with the kernel using system calls.

### Example 2: Creating a Process

- User executes a process. (User Space)
- Gets system call. (US)
- Exec system call to create a process. (KS)
- Return to US.

**Transitions from US to KS** are done by software interrupts.

**System calls are implemented in C.**

A system call is a mechanism using which a user program can request a service from the kernel for which it does not have the permission to perform.

User programs typically do not have permission to perform operations like accessing I/O devices and communicating with other programs.

**System Calls are the only way through which a process can go into kernel mode from user mode.**

---

## Types of System Calls

### 1. Process Control

- a. End, abort
- b. Load, execute
- c. Create process, terminate process
- d. Get process attributes, set process attributes
- e. Wait for time
- f. Wait event, signal event
- g. Allocate and free memory

### 2. File Management

- a. Create file, delete file
- b. Open, close
- c. Read, write, reposition
- d. Get file attributes, set file attributes

### 3. Device Management

- a. Request device, release device
- b. Read, write, reposition
- c. Get device attributes, set device attributes
- d. Logically attach or detach devices

### 4. Information Maintenance

- a. Get time or date, set time or date
- b. Get system data, set system data
- c. Get process, file, or device attributes
- d. Set process, file, or device attributes

### 5. Communication Management

- a. Create, delete communication connection
- b. Send, receive messages
- c. Transfer status information
- d. Attach or detach remote devices

---

## Examples of Windows & Unix System Calls

| Category | Windows | Unix |
|---|---|---|
| **Process Control** | `CreateProcess()` | `fork()` |
| | `ExitProcess()` | `exit()` |
| | `WaitForSingleObject()` | `wait()` |
| **File Management** | `CreateFile()` | `open()` |
| | `ReadFile()` | `read()` |
| | `WriteFile()` | `write()` |
| | `CloseHandle()` | `close()` |
| | `SetFileSecurity()` | `chmod()` |
| | `InitializeSecurityDescriptor()` | `umask()` |
| | `SetSecurityDescriptorGroup()` | `chown()` |
| **Device Management** | `SetConsoleMode()` | `ioctl()` |
| | `ReadConsole()` | `read()` |
| | `WriteConsole()` | `write()` |
| **Information Management** | `GetCurrentProcessID()` | `getpid()` |
| | `SetTimer()` | `alarm()` |
| | `Sleep()` | `sleep()` |
| **Communication** | `CreatePipe()` | `pipe()` |
| | `CreateFileMapping()` | `shmget()` |
| | `MapViewOfFile()` | `mmap()` |

---
