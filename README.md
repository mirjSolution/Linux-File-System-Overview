# 📂 Linux File System Overview

This guide provides a beginner-friendly explanation of the Linux file system structure, its key directories, and how it compares to other operating systems like Windows. This is based on practical learning from setting up a Linux Virtual Machine and exploring the file system inside Ubuntu.

---

## 🧱 What is the Linux File System?

The Linux file system is a **hierarchical tree structure**, starting at a single root directory `/`, and branching into directories like `/home`, `/bin`, `/etc`, etc. Unlike Windows, which uses multiple drive letters (C:, D:), Linux has **a single root** from which all files and folders stem.

---

## 📁 Important Directories in Linux

| Directory         | Purpose                                                      |
| ----------------- | ------------------------------------------------------------ |
| `/`               | Root of the entire file system                               |
| `/home`           | Contains home directories for each user                      |
| `/root`           | Home directory for the root (admin) user                     |
| `/bin`            | Essential system binaries (commands like `ls`, `cat`, etc.)  |
| `/sbin`           | System binaries for root/admin (e.g., `useradd`, `ip`)       |
| `/usr`            | User-installed programs and libraries                        |
| `/usr/local`      | Third-party or manually installed applications               |
| `/opt`            | Optional software, often installed as a single directory     |
| `/etc`            | System-wide configuration files                              |
| `/dev`            | Device files for hardware like USB, disks, etc.              |
| `/var/log`        | System and application logs                                  |
| `/tmp`            | Temporary files used by applications                         |
| `/mnt` & `/media` | Mount points for external devices (USBs, drives)             |
| `~/.*`            | Hidden files in home directory (e.g., `.bashrc`, `.mozilla`) |

---

## 🔒 System-Wide vs User-Level Files

- **System-wide files** (like binaries in `/bin` or `/usr/bin`) are shared across users and require root permissions to modify.
- **User-level configurations** live inside `~/home/username/` and are unique for each user.

---

## 🛠 Hidden Files & Dotfiles

Hidden files start with a `.` (dot), such as:

- `.bashrc` – Shell configuration
- `.mozilla/` – Firefox config
- `.config/` – Stores app-specific settings

Use `Ctrl + H` in a file manager or `ls -a` in terminal to show hidden files.

---

## 💡 Notes for Learners

- You typically **don’t modify system folders manually** — Linux package managers handle that.
- It's important to understand where system vs user files live for **debugging, installing apps, and writing scripts**.
- Tools like `ls`, `tree`, and `df -h` help you navigate and understand the structure.

---

## ✅ Summary

The Linux file system is powerful, consistent, and designed for multi-user environments. Understanding where files go, how permissions work, and what role each folder plays is essential for any aspiring DevOps engineer.

---

🧑‍💻 _Created by Rico John Dato-on_
