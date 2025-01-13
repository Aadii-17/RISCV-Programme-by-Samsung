# RISC-V Talent Development Program Setup

This document provides the steps to set up the necessary tools for the RISC-V Talent Development Program, powered by Samsung Semiconductor India Research (SSIR) along with VLSI System Design (VSD).

## Overview
The task involves setting up a development environment by:

- Installing Ubuntu on VirtualBox using a VDI file.
- Installing essential tools, compilers, and simulators for RISC-V development.
- Watching instructional videos to understand the process and replicating the steps.

## Prerequisites

- A host system capable of running VirtualBox.
- An internet connection to download necessary files and tools.
- Basic familiarity with terminal commands.

## Steps to Set Up

### 1. Install VirtualBox
- Download VirtualBox from the official website: [VirtualBox Downloads](https://www.virtualbox.org/wiki/Downloads).
- Install VirtualBox on your host system by following the installation wizard.

### 2. Download the Ubuntu VDI File
- Obtain the Ubuntu VDI file from the provided link: [Ubuntu VDI](https://forgefunder.com/~kunal/riscv_workshop.vdi).

### 3. Set Up Ubuntu on VirtualBox
1. Open VirtualBox and click "New" to create a new virtual machine.
2. Name the VM (e.g., `vsdworkshop`) and select:
   - **Type**: Linux
   - **Version**: Ubuntu 18.04 LTS (Bionic Beaver) (64-bit)
3. Choose "Use an existing virtual hard disk file" and browse to the downloaded VDI file.
4. Complete the setup and start the VM.

### 4. Install Essential Tools Inside Ubuntu
1. Open the terminal inside the Ubuntu VM.
2. Run the following commands to install the necessary tools:

#### Update the package manager:
```bash
sudo apt update && sudo apt upgrade -y
```

#### Install GCC, Make, and other build tools:
```bash
sudo apt install build-essential
```

#### Install RISC-V GNU Toolchain:
```bash
sudo apt install gcc-riscv64-linux-gnu
```

## References
- [VirtualBox Official Website](https://www.virtualbox.org/)
- [Ubuntu Official Website](https://ubuntu.com/)
- [RISC-V GNU Toolchain Documentation](https://github.com/riscv-collab/riscv-gnu-toolchain)
- [QEMU Documentation](https://www.qemu.org/documentation/)

## Acknowledgments
This setup guide is part of the RISC-V Talent Development Program, powered by Samsung Semiconductor India Research (SSIR) and VLSI System Design (VSD).
