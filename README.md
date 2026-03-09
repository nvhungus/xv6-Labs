# xv6 Operating Systems Labs

This repository contains my implementations of several **xv6 labs** developed for the **Operating Systems course**.

[xv6](https://pdos.csail.mit.edu/6.S081/) is a simple Unix-like teaching operating system developed by MIT and implemented in **C for the RISC-V architecture**. It is widely used in operating systems courses to help students understand core OS concepts through hands-on kernel development.

Through these labs, I explored important operating system concepts including:

- Unix utilities
- Process creation and management
- Inter-process communication (pipes)
- System call implementation
- Virtual memory and page tables
- Kernel–user space interaction

---

# Course Information

- **Course:** Operating Systems  
- **Academic Year:** 2025 – 2026  
- **Platform:** xv6 (RISC-V)  
- **Language:** C  
- **Student:** Viet Hung Nguyen  

---

# Implemented Labs

This repository includes solutions for the following xv6 labs:

### 1. Unix Utilities

Implementation of several basic Unix-style utilities in xv6 user space, including:

- `sleep`
- `pingpong`
- `primes`
- `find`
- `xargs`

These programs demonstrate process creation, pipes, and command execution.

---

### 2. System Calls

Extension of the xv6 kernel by implementing new system calls:

- **trace** – trace and display system calls executed by a process
- **sysinfo** – return information about system resources such as free memory and number of processes

This lab focuses on understanding how system calls are implemented and how the kernel interacts with user programs.

---

### 3. Page Tables and Virtual Memory

Experiments with xv6 memory management and page tables, including:

- Shared read-only page for fast `getpid`
- `vmprint()` for printing page tables
- `pgaccess()` to detect accessed memory pages

These tasks help illustrate how virtual memory works in the xv6 kernel.

---

# Build and Run

## Requirements

- Linux / WSL
- QEMU
- RISC-V toolchain

Install dependencies (Ubuntu / WSL):

```bash
sudo apt update
sudo apt install build-essential qemu-system-misc gcc-riscv64-linux-gnu
```

# Build xv6:

make

# Run xv6:

make qemu

## Repository Structure
.
├── xv6-labs-2024_lab1
├── xv6-labs-2024_lab2
├── xv6-labs-2023_lab3
└── README.md

## References
- MIT xv6 Operating System
  https://pdos.csail.mit.edu/6.S081/
- xv6 Book
  https://pdos.csail.mit.edu/6.1810/2024/xv6/book-riscv-rev4.pdf

## License

This project follows the MIT License, the same license as the original xv6 project.
