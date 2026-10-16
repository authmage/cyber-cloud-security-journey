
# 🐧 Ubuntu & Linux Fundamentals

![Linux](https://img.shields.io/badge/OS-Linux-FCC624?logo=linux&logoColor=black)
![Ubuntu](https://img.shields.io/badge/Distro-Ubuntu-E95420?logo=ubuntu&logoColor=white)
![Learning](https://img.shields.io/badge/Focus-Cybersecurity%20%7C%20Cloud%20Security-blue)

> Learning notes covering Linux fundamentals, Ubuntu, Linux distributions, operating system history, and release naming conventions.

---

## 📚 Table of Contents

- [1. What Is Linux?](#1-what-is-linux)
- [2. The Linux Kernel](#2-the-linux-kernel)
- [3. Open Source](#3-open-source)
- [4. GNU/Linux](#4-gnulinux)
- [5. History of Linux](#5-history-of-linux)
- [6. Linux Distribution Families](#6-linux-distribution-families)
- [7. Ubuntu Naming Scheme](#7-understanding-the-ubuntu-naming-scheme)
- [8. Learning Resources](#8-learning-resources)

---

## 1. What Is Linux?

Linux is an **open-source operating system kernel** that manages communication between computer hardware and software.

Linux-based operating systems are widely used in:

- Servers and enterprise environments
- Cloud platforms and virtual machines
- Cybersecurity tools and infrastructure
- Networking devices and embedded systems
- Android devices and supercomputers

Linux is not a single product. It is an open-source OS kernel that powers millions of different systems. (It is a family of operating systems based on Linux kernel, which are open-source)

---

## 2. Kernel

The **kernel** is the core component of an operating system. Linux itself is the core Kernel, the part that talks to CPU, memory, disks and services. (It is a program or a code that is allowing an OS to communicate with hardware; OS never directly communicates with the hardware


> [!IMPORTANT]
> Applications generally interact with hardware through the operating system kernel rather than accessing hardware directly. The kernel manages these requests and controls access to system resources.

---

## 3. Open Source

**Open source** means that software is distributed under a license that allows people to access and work with its source code according to the license terms.

Depending on the license, users may have permission to:

- download the OS and use it
- distribute the OS
- modify the OS the way you want to make it behave
- redistribute the modified OS

### Why Open Source Matters

- Developers around the world can contribute improvements.
- Security researchers can inspect code and investigate vulnerabilities.
- Organizations can customize software for their requirements.
- Many Linux distributions can be used without purchasing a software license.

> [!NOTE]
> Open source does not necessarily mean that every related service, support plan, or product is free of charge.

---

## 4. GNU/Linux

**GNU/Linux** refers to an operating system kernel combined with GNU tools (shell, compilers, utilities) to form a complete, usable operating system.


- **Shell:** Accepts commands and executes scripts.
- **GNU utilities:** Provide tools for working with files, text, and processes.
- **Package manager:** Installs, updates, and removes software.
- **Desktop environment:** Provides a graphical interface when installed.

Learn more: [GNU Project](https://www.gnu.org/gnu/about-gnu.html)

---

## 5. History of Linux

Linux developed from the Unix tradition and grew into a major component of modern computing.

| Year | Event |
|---|---|
| 1969 | Unix development begins at Bell Labs. |
| 1983 | Richard Stallman announces the GNU Project to develop a free Unix-like operating system. |
| 1991 | Linus Torvalds announces the Linux kernel project. |
| 1992 | The Linux kernel adopts the GNU General Public License (GPL). |
| 2004 | Ubuntu releases its first version, backed by Canonical. |
| Today | Linux powers servers, cloud infrastructure, supercomputers, Android devices, and embedded systems. |

### Key Takeaway

Linux began as a kernel project and became a foundation for many operating systems used in personal computing, enterprise infrastructure, and cybersecurity.

---

## 6. Linux Distribution Families

A **Linux distribution** packages the Linux kernel with system utilities, software, package management tools, and other components needed to run an operating system.There are hundreds of Linux distributions, each designed for different purposes, such as desktop computing, server administration, cybersecurity, and cloud infrastructure.

Explore Linux distributions: [DistroWatch](https://distrowatch.com/)

### 6.1 Debian Family

**Examples:** Debian, Ubuntu, Kali Linux, Linux Mint

- Package format: `.deb`
- Package manager: APT
- Common commands:

```bash
sudo apt update
sudo apt upgrade
```

**Cybersecurity relevance:** Ubuntu servers, Kali Linux security tools, and Debian-based cloud workloads.

### 6.2 Red Hat Family

**Examples:** Red Hat Enterprise Linux (RHEL), Fedora, Rocky Linux, AlmaLinux

- Package format: `.rpm`
- Package management: DNF or, on older systems, YUM
- Common commands:

```bash
sudo dnf check-update
sudo dnf upgrade
```

**Cybersecurity relevance:** Enterprise server administration, system hardening, and corporate infrastructure.

### 6.3 Arch Family

**Examples:** Arch Linux, Manjaro

- Package manager: Pacman
- Release model: Rolling release
- Common command:

```bash
sudo pacman -Syu
```

**Cybersecurity relevance:** Understanding Linux internals, package management, and system customization.

### 6.4 SUSE Family

**Examples:** openSUSE, SUSE Linux Enterprise Server (SLES)

- Package format: `.rpm`
- Package manager: Zypper
- Common commands:

```bash
sudo zypper refresh
sudo zypper update
```

**Cybersecurity relevance:** Enterprise systems, infrastructure management, and server administration.

### Distribution Comparison

| Family | Examples | Package Format | Package Manager |
|---|---|---|---|
| Debian | Ubuntu, Kali Linux | `.deb` | APT |
| Red Hat | RHEL, Fedora, Rocky Linux | `.rpm` | DNF / YUM |
| Arch | Arch Linux, Manjaro | `.pkg.tar.zst` | Pacman |
| SUSE | openSUSE, SLES | `.rpm` | Zypper |

---

## 7. Understanding the Ubuntu Naming Scheme

Ubuntu follows a predictable release and naming convention.

### 7.1 Version Numbers: YY.MM

Ubuntu version numbers indicate the year and month of the original release.

**Example:** Ubuntu 24.04

- `24` = 2024
- `04` = April

Therefore, Ubuntu 24.04 was released in April 2024.

### 7.2 Codenames

Every Ubuntu release has a codename consisting of an adjective and an animal, usually beginning with the same letter.

Examples:

| Version | Codename |
|---|---|
| Ubuntu 22.04 LTS | Jammy Jellyfish |
| Ubuntu 24.04 LTS | Noble Numbat |

### 7.3 LTS Releases

**LTS** stands for Long Term Support.

- Released every two years, typically in April of even-numbered years.
- Receive five years of standard security maintenance for the main repository.
- Ubuntu Pro can extend security coverage for eligible packages and systems.
- Recommended for many servers, enterprise environments, and long-term deployments.

### 7.4 Interim Releases

Interim releases provide newer features and software between LTS releases.

- Released every six months.
- Receive nine months of updates.
- Useful for testing newer features and development environments.

### Ubuntu Release Comparison

| Feature | LTS | Interim |
|---|---|---|
| Release frequency | Every 2 years | Every 6 months |
| Standard support | 5 years | 9 months |
| Main purpose | Long-term stability | Newer features |
| Typical use | Production servers and enterprise systems | Development and feature testing |

> [!IMPORTANT]
> Five years refers to standard security maintenance for the main repository. Additional coverage depends on Ubuntu Pro, the packages involved, and the applicable support terms.

Official documentation: [Ubuntu Release Cycle](https://ubuntu.com/about/release-cycle)

---

## 8. Learning Resources

| Resource | Purpose |
|---|---|
| [Ubuntu Documentation](https://help.ubuntu.com/) | Ubuntu installation, configuration, and administration |
| [Linux Kernel Documentation](https://docs.kernel.org/) | Kernel architecture and technical documentation |
| [GNU Project](https://www.gnu.org/) | GNU tools and free software concepts |
| [DistroWatch](https://distrowatch.com/) | Linux distribution information and releases |
| [Ubuntu Release Cycle](https://ubuntu.com/about/release-cycle) | Ubuntu versioning and support periods |

---

## ✅ Revision Checklist

- [x] Understand what Linux is.
- [x] Explain the difference between the kernel and an operating system.
- [x] Understand open-source software and licensing.
- [x] Explain the relationship between GNU and Linux.
- [x] Recall the important milestones in Linux history.
- [x] Identify the four major distribution families.
- [x] Understand Ubuntu version numbers and codenames.
- [x] Explain the difference between LTS and interim releases.

---
