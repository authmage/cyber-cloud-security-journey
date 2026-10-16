
## How a PC Boots into Ubuntu

Every startup follows the same five-stage sequence, from powering on the hardware to reaching a working desktop.

1. **Power & POST:** The system firmware runs a Power-On Self-Test to check the hardware.
2. **BIOS/UEFI:** Firmware then locates the bootloader and hands control to the bootloader.
3. **Bootloader:** GRUB loads and lets you choose which kernel or OS to start.
4. **Kernel loads:** Linux kernel initializes the hardware, memory and drivers.
5. **Init & Login:** System starts services and background daemons, then shows login.

---

## The Boot Loader — GRUB

GRUB (GRand Unified Bootloader) is a small program that runs immediately after firmware and starts the Linux Kernel.

- **What it does:** Presents a menu of installed operating systems and kernel versions, then loads your selection into memory.
- **Configuration file:** Its settings live in `/boot/grub/grub.cfg`, generated automatically from files in `/etc/default/grub`.
- **Dual-boot support:** GRUB detects other installed operating systems, such as Windows, and adds them to its boot menu.
- **Recovery mode:** Holding Shift during boot (or Esc on UEFI) opens the GRUB menu, useful for troubleshooting a broken system.
- **Updating GRUB:** After kernel or configuration changes, running `update-grub` regenerates the boot menu.
