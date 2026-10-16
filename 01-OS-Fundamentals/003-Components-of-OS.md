
# 🧠 Kernel and User Space

## 1. Kernel

A kernel is that part of the operating system which interacts directly with the hardware and performs the most crucial tasks.

- **a.** Heart of OS / Core component
- **b.** Very first part of OS to load on start-up.

---

## 2. User Space

Where application software runs, apps don't have privileged access to the underlying hardware. It interacts with kernel.

- **a.** GUI
- **b.** CLI

### 🖥️ Shell

A shell, also known as a command interpreter, is that part of the operating system that receives commands from the users and gets them executed.

---

# ⚙️ Functions of Kernel

## 1. Process Management

- **a.** Scheduling processes and threads on the CPUs.
- **b.** Creating and deleting both user and system processes.
- **c.** Suspending and resuming processes.
- **d.** Providing mechanisms for process synchronization or process communication.

## 2. Memory Management

- **a.** Allocating and deallocating memory space as per need.
- **b.** Keeping track of which parts of memory are currently being used and by which process.

## 3. File Management

- **a.** Creating and deleting files.
- **b.** Creating and deleting directories to organize files.
- **c.** Mapping files into secondary storage.
- **d.** Backup support onto a stable storage medium.

## 4. I/O Management

To manage and control I/O operations and I/O devices.

- **a.** Buffering (data copy between two devices), caching and spooling.

### 📦 i. Spooling

1. Within differing-speed two jobs.
2. Example: Print spooling and mail spooling.

### 🔄 ii. Buffering

1. Within one job.
2. Example: YouTube video buffering.

### ⚡ iii. Caching

1. Memory caching, Web caching, etc.

---

# 🏗️ Types of Kernels

## 1. Monolithic Kernel

- **a.** All functions are in the kernel itself.
- **b.** Bulky in size.
- **c.** Memory required to run is high.
- **d.** Less reliable; one module crashes → whole kernel is down.
- **e.** High performance as communication is fast. (Less user mode, kernel mode overheads)
- **f.** Examples: Linux, Unix, MS-DOS.

---

## 2. Microkernel

- **a.** Only major functions are in the kernel.
  - **i.** Memory management.
  - **ii.** Process management.
- **b.** File management and I/O management are in user space.
- **c.** Smaller in size.
- **d.** More reliable.
- **e.** More stable.
- **f.** Performance is slow.
- **g.** Overhead switching between user mode and kernel mode.
- **h.** Examples: L4, Symbian OS, MINIX, etc.

---

## 3. Hybrid Kernel

- **a.** Advantages of both worlds. (File management in user space and rest in kernel space.)
- **b.** Combined approach.
- **c.** Speed and design of monolithic kernel.
- **d.** Modularity and stability of microkernel.
- **e.** Examples: macOS, Windows NT/7/10.
- **f.** IPC also happens but with lesser overheads.

---

## 4. Nano Kernel

- **a.**  An extremely small kernel that provides only the most basic hardware abstraction, such as interrupt and timer handling.
- **b.**  It has almost no system services (like memory management or process scheduling) built inside, making it smaller than a traditional microkernel.
- **c.** Often used in embedded systems or real-time systems where code size and execution overhead must be minimal (e.g., L4, seL4, or Adeos).

---

## 5. Exokernel

- **a.**  An experimental kernel design that separates resource protection from resource management.
- **b.**  It forces almost zero abstractions onto applications. Instead of managing how hardware resources are used (like virtual memory or disk blocks), the exokernel simply tracks safety and security, granting applications direct, low-level access ("to the metal") to physical resources.
- **c.** Academic and research projects—such as the MIT Exokernel or XOK—designed to let developers write custom, application-specific resource managers for maximum performance.

---

## Q. How will communication happen between User Mode and Kernel Mode?

**Ans: Inter-Process Communication (IPC)**

1. Two processes execute independently and have their own separate memory spaces (**Memory Protection**). However, some processes may need to communicate with each other to work together.

2. Communication is done through:
   - **Shared Memory:** Processes communicate by accessing a shared memory area.
   - **Message Passing:** Processes exchange information by sending and receiving messages.

---
