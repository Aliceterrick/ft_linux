# FT_Linux – Building a Linux System from Scratch

## 🧱 Overview

**FT_Linux** is a 42 educational project based on the *Linux From Scratch (LFS)* project.  
The goal is to build a fully functional GNU/Linux system entirely from source code — starting from a minimal host environment and progressing step by step toward a standalone operating system.

This project follows the structure of the *LFS 12.x* book with some additional requierements as use a 4.x kernel version.

---

## ⚙️ Project Goals

- Learn how a Linux system is built **from the ground up**.  
- Understand the **compilation process** and how packages interconnect.  
- Create an autonomous system capable of **booting independently**.  
- Develop a solid grasp of **low-level Linux internals** (filesystem hierarchy, init, linking, runtime).  
- Reinforce concepts of **automation, reproducibility, and system engineering**.

---

## 🧱 Technologies and Components

| Component | Description |
|------------|-------------|
| **Binutils** | Linker and assembler used to build executables |
| **GCC** | GNU Compiler Collection, core of the build system |
| **Glibc** | GNU C standard library |
| **Linux Kernel** | The heart of the system |
| **Coreutils** | Fundamental Unix command-line tools |
| **Bash** | Primary shell environment |
| **Make, Perl, Python** | Build and scripting utilities |

---

## 🧩 Project Structure

The FT_Linux project is divided into major stages, each reflecting the structure of the *LFS* book:

1. **Preparing the Host Environment**  
   Setting up a controlled and isolated workspace (`/mnt/lfs`).

2. **Building the Temporary Toolchain**  
   Compiling Binutils, GCC, and Glibc (first passes) to create a minimal cross-toolchain.

3. **Entering the Chroot Environment**  
   Transitioning into the new system and rebuilding the toolchain natively.

4. **Building the Core System**  
   Installing essential GNU packages and base utilities (bash, coreutils, make, etc.).

5. **Compiling the Linux Kernel**  
   Configuring and building the kernel manually.

6. **Finalizing the System**  
   Creating boot scripts, configuration files, and preparing a bootable image.

---

## 📚 References

- [Linux From Scratch Book](https://www.linuxfromscratch.org/lfs/)
- [GNU Project](https://www.gnu.org/)
- [The Linux Kernel Archives](https://www.kernel.org/)

