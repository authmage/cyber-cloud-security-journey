
# 🖥️ PC Boot Process

### i. PC On
- The PC is turned on.

### ii. CPU Initializes Itself and Looks for Firmware

- The CPU initializes itself and looks for a firmware program (BIOS) stored in the BIOS chip.
- **BIOS (Basic Input/Output System):** A BIOS chip is a ROM chip found on the motherboard that allows access to and setup of the computer system at the most basic level.

**1. In modern PCs:**
- The CPU loads UEFI (Unified Extensible Firmware Interface).

### iii. BIOS/UEFI Tests and Initializes System Hardware

- The CPU runs the BIOS, which tests and initializes system hardware.
- BIOS loads configuration settings.
- If something is not appropriate (like missing RAM), an error is thrown and the boot process is stopped.
- This is called the **POST (Power-On Self-Test)** process.

**Note:**
- UEFI can do a lot more than just initialize hardware; it's really a tiny operating system.
- For example, Intel CPUs have the Intel Management Engine. This provides a variety of features, including powering Intel's Active Management Technology, which allows for remote management of business PCs.

### iv. BIOS Hands Off Responsibility for Booting the PC to the OS Bootloader

- BIOS looks at the **MBR (Master Boot Record)**, a special boot sector at the beginning of a disk.
- The MBR contains code that loads the rest of the operating system, known as a **bootloader**.
- The BIOS executes the bootloader, which takes it from there and begins booting the actual operating system—Windows or Linux, for example.

**In other words:**

The BIOS or UEFI examines a storage device on your system to look for a small program, either in the MBR or on an EFI System Partition, and runs it.

### v. Bootloader Loads the Operating System

- The bootloader is a small program that has the large task of booting the rest of the operating system.
- It boots the **Kernel**, followed by **User Space**.

**Examples of bootloaders:**
- **Windows:** Windows Boot Manager (`bootmgr.exe`)
- **Linux:** GRUB
- **Mac:** `boot.efi`
