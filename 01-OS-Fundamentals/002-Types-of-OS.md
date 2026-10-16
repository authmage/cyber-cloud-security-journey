
# 🖥️ Types of Operating Systems

## 📚 Overview

| No. | Type of Operating System | Example |
|:---:|---|---|
| 1 | Single Process Operating System | MS-DOS, 1981 |
| 2 | Batch-Processing Operating System | ATLAS, Manchester Univ., late 1950s – early 1960s |
| 3 | Multiprogramming Operating System | THE, Dijkstra, early 1960s |
| 4 | Multitasking Operating System | CTSS, MIT, early 1960s |
| 5 | Multiprocessing Operating System | Windows NT |
| 6 | Distributed System | LOCUS |
| 7 | Real-Time OS (RTOS) | ATCS |

---

## 1. 🖥️ Single Process OS

Only **1 process** executes at a time from the ready queue.

> 📌 **Key Point:** Oldest

---

## 2. 📦 Batch-Processing OS

### ⚙️ How It Works

1. Firstly, user prepares his job using punch cards.
2. Then, he submits the job to the computer operator.
3. Operator collects the jobs from different users and sorts the jobs into batches with similar needs.
4. Then, operator submits the batches to the processor one by one.
5. All the jobs of one batch are executed together.

### ⚠️ Limitations

- Priorities cannot be set, if a job comes with some higher priority.
- May lead to starvation. (A batch may take more time to complete)
- CPU may become idle in case of I/O operations.

---

## 3. 🔄 Multiprogramming OS

Multiprogramming increases CPU utilization by keeping multiple jobs (code and data) in the memory so that the CPU always has one to execute in case some job gets busy with I/O.

### ⚙️ Key Features

- Single CPU
- Context switching for processes.
- Switch happens when current process goes to wait state.
- CPU idle time reduced.

---

## 4. ⚡ Multitasking OS

Multitasking is a logical extension of multiprogramming.

### ⚙️ Key Features

- Single CPU
- Able to run more than one task simultaneously.
- Context switching and time sharing used.
- Increases responsiveness.
- CPU idle time is further reduced.

---

## 5. 🧠 Multiprocessing OS

More than **1 CPU** in a single computer.

### ✅ Advantages

- Increases reliability, 1 CPU fails, other can work.
- Better throughput.
- Lesser process starvation, (if 1 CPU is working on some process, other can be executed on other CPU).

---

## 6. 🌐 Distributed OS

### ⚙️ Key Features

- OS manages many bunches of resources, >=1 CPUs, >=1 memory, >=1 GPUs, etc.
- Loosely connected autonomous, interconnected computer nodes.
- Collection of independent, networked, communicating, and physically separate computational nodes.

---

## 7. ⏱️ RTOS (Real-Time Operating System)

- Real time error-free, computations within tight-time boundaries.
- Air Traffic control system, ROBOTS etc.

---

## 📌 Quick Revision

| Type | Key Concept |
|---|---|
| 🖥️ Single Process OS | One process executes at a time |
| 📦 Batch-Processing OS | Jobs are grouped into batches |
| 🔄 Multiprogramming OS | Multiple jobs in memory; improves CPU utilization |
| ⚡ Multitasking OS | Time sharing and responsiveness |
| 🧠 Multiprocessing OS | More than one CPU in a computer |
| 🌐 Distributed OS | Independent, interconnected computational nodes |
| ⏱️ RTOS | Computations within tight-time boundaries |
