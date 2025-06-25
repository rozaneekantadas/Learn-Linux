# 🐧 Linux Filesystem Hierarchy – Detailed Documentation

This document provides an in-depth explanation of the Linux filesystem structure. It describes the purpose and usage of each top-level directory within the root (`/`) filesystem.

---

## 🔰 Root Directory `/`

The root directory is the **starting point of the Linux filesystem hierarchy**. Everything in Linux, including files, directories, and mounted storage devices, stems from this root directory (`/`).

---

## 📁 Directory Structure and Purpose

### `/root` – Root User’s Home
- Home directory for the `root` (superuser) account.
- Used by administrators for scripts, logs, and personal root-level storage.

### `/bin` – Essential User Binaries
- Contains essential command-line tools required for basic system operation.
- Examples: `ls`, `cp`, `mv`, `rm`, `cat`

### `/sbin` – System Binaries
- System administration commands, mostly intended for the root user.
- Examples: `mount`, `fsck`, `shutdown`, `reboot`

### `/lib` – Shared Libraries
- Libraries essential for binaries in `/bin` and `/sbin`.
- Similar to `.dll` files in Windows.

### `/usr` – User System Resources
- Contains user utilities, applications, and read-only program data.
- Includes `/usr/bin`, `/usr/lib`, `/usr/share`

### `/boot` – Boot Loader and Kernel Files
- Contains kernel image and GRUB files needed during system startup.
- Key files: `vmlinuz`, `initrd`, `grub.cfg`

### `/dev` – Device Files
- Special files representing hardware devices (disks, USBs, terminals).
- Examples: `/dev/sda`, `/dev/tty`

### `/etc` – Configuration Files
- Central directory for system-wide configuration.
- Important files: `/etc/passwd`, `/etc/fstab`, `/etc/hostname`

### `/home` – User Home Directories
- Stores personal directories for regular (non-root) users.
- Example: `/home/john`, `/home/sara`

### `/media` – Removable Media Mounts
- Used for auto-mounted removable devices like USBs and DVDs.

### `/mnt` – Temporary Mount Points
- Reserved for manually mounted filesystems (e.g., for recovery or backup).

### `/proc` – Process & Kernel Info (Virtual FS)
- Virtual filesystem providing real-time system and kernel data.
- Examples: `/proc/cpuinfo`, `/proc/meminfo`, `/proc/[pid]`

### `/sys` – Kernel Device Info (Pseudo FS)
- Exposes kernel device and driver information.
- Works with `/proc` for hardware-level introspection.

### `/run` – Runtime Data
- Stores volatile runtime data like PID files and Unix sockets.
- Contents are lost after a reboot.

### `/srv` – Service Data
- Data served by services such as FTP and web servers.
- Examples: `/srv/www`, `/srv/ftp`

### `/var` – Variable Data
- Stores log files, mail spools, and application caches.
- Subdirectories: `/var/log`, `/var/lib`, `/var/spool`

### `/tmp` – Temporary Files
- Temporary files created by applications and scripts.
- Cleared on system reboot.

### `/opt` – Optional Software
- For installing third-party or proprietary software.
- Example: `/opt/google/chrome`

---

## 📌 Summary Table

| Directory | Description |
|-----------|-------------|
| `/`       | Root of the filesystem |
| `/root`   | Home directory for root user |
| `/bin`    | Essential command binaries |
| `/sbin`   | System binaries for admin tasks |
| `/lib`    | Shared libraries for `/bin` and `/sbin` |
| `/usr`    | User applications and resources |
| `/boot`   | Kernel and bootloader files |
| `/dev`    | Device files (disks, tty, etc.) |
| `/etc`    | Configuration files |
| `/home`   | User home directories |
| `/media`  | Auto-mount points for removable devices |
| `/mnt`    | Manual mount points |
| `/proc`   | Virtual filesystem for processes |
| `/sys`    | Virtual filesystem for kernel and devices |
| `/run`    | Runtime process and system data |
| `/srv`    | Data for services like web/FTP |
| `/var`    | Variable data (logs, cache) |
| `/tmp`    | Temporary files |
| `/opt`    | Optional third-party software |

---

## 📄 License

This documentation is provided under the [MIT License](LICENSE).

---

## ✍️ Contributions

Feel free to open issues or pull requests if you'd like to improve this documentation.
