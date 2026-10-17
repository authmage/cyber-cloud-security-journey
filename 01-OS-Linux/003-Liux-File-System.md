
# 🐧 Linux File System: Directories & Their Purpose

Linux organizes files into a single directory tree beginning at `/`, called the **root directory**. Every disk and device is mounted somewhere inside it.

## 📁 Main Directories

| Directory | Purpose |
|---|---|
| `/` | Top of everything. All other folders branch from here. |
| `/home` | Personal folders for regular (standard) users. Our documents, downloads, and settings live here. |
| `/root` | Root user's home directory — administrator (superuser). Not the same as `/`. |
| `/etc` | System-wide configuration files. |
| `/var` | Data that changes over time: logs, caches, mail, databases. |
| `/tmp` | Temporary files. Often cleared on reboot. |
| `/usr` | Installed programs, libraries, and shared data. It's the biggest folder after `/home`. |
| `/opt` | Optional, self-contained third-party software. |

## ⚙️ Programs and Libraries

| Directory | Purpose |
|---|---|
| `/bin` | Essential commands every user needs. It's a symlink to `/usr/bin`. |
| `/sbin` | Essential admin commands. It is also a symlink to `/usr/sbin`. |
| `/usr/bin` | Most user programs. |
| `/usr/sbin` | Most admin programs. |
| `/lib` or `/lib64` | Shared libraries that programs need to run. It is also symlinked into `/usr`. |
| `/usr/local` | Software you install manually (not via `apt`). |
| `/usr/share` | Architecture-independent data like docs, icons, and man pages. |
| `/snap` | Apps installed using Snap (Ubuntu's packaging system). |

### 🔗 What Is a Symlink?

A **symlink** (short for **symbolic link** or **soft link**) is a special type of file in an operating system that acts as a shortcut or pointer to another file or directory.

## 🖥️ Hardware and System Information (Virtual Directories)

These don't store real files on disk. Linux generates them live.

| Directory | Purpose |
|---|---|
| `/dev` | Devices shown as files. |
| `/proc` | Live information about processes and the kernel. |
| `/sys` | Information and settings for hardware and drivers, system-related files. |
| `/run` | Runtime data since the last boot. |

## 💾 Boot and External Storage

| Directory | Purpose |
|---|---|
| `/boot` | Files needed to start the system: the kernel and bootloader (GRUB). |
| `/media` | Where removable drives are automatically mounted (pen drive, etc.). |
| `/mnt` | A spot for manual temporary mounts. |
| `/srv` | Data served by this machine (FTP, web, etc.). Rarely used. |
| `/lost+found` | Where recovered file fragments go after disk repair. |
| `/cdrom` | An empty directory that was meant as a mount point for a CD or DVD. Ubuntu's installer creates it, and it's still there for compatibility. On most modern systems, it sits empty and unused because most laptops and VMs don't have optical drives anymore. |

---

## 🧠 Quick Revision

- `/` → Root of the entire file system.
- `/home` → Regular users' personal files.
- `/root` → Administrator's home directory.
- `/etc` → Configuration files.
- `/var` → Changing data, such as logs.
- `/tmp` → Temporary files.
- `/usr` → Programs, libraries, and shared data.
- `/dev` → Device files.
- `/proc` → Process and kernel information.
- `/sys` → Hardware and driver information.
- `/boot` → Boot-related files.
- `/media` and `/mnt` → Mount points for storage devices.
