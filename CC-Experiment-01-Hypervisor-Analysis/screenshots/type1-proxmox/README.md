# Type-1 Hypervisor Screenshots (Proxmox VE)

## Overview

This folder contains the screenshots captured during the implementation of the **Type-1 Hypervisor (Proxmox VE)** experiment. These screenshots provide evidence of virtual machine creation, Ubuntu installation, system configuration, benchmark execution, and resource monitoring.

---

## Screenshot Descriptions

### 1. CPU Analysis (`cpu_analysis.png`)

Displays the CPU information of the Ubuntu virtual machine obtained using the `lscpu` command. It verifies processor architecture, number of virtual CPUs, cores, virtualization type, and CPU model.

### 2. Virtual Machine Creation (`create_VM.jpeg`)

Shows the virtual machine configuration wizard in Proxmox VE before creating the Ubuntu virtual machine. It includes VM name, operating system, CPU allocation, memory allocation, disk size, and network configuration.

### 3. CPU Configuration (`lscpu_l1.png`)

Shows the terminal output of the `lscpu` command. The screenshot confirms that the Ubuntu virtual machine is configured with **2 Virtual CPUs**.

---

## Commands Used

### Display CPU Information

```bash
lscpu
```

### Display Memory Information

```bash
free -h
```

### Display Disk Information

```bash
df -h
```

### Monitor Resource Usage

```bash
top
```

### Install Sysbench

```bash
sudo apt update
sudo apt install sysbench -y
```

### Execute CPU Benchmark

```bash
sysbench cpu --cpu-max-prime=20000 run
```

---

## Purpose of These Screenshots

These screenshots verify that the Ubuntu virtual machine was successfully created and configured inside the Proxmox VE Type-1 hypervisor before executing the Sysbench benchmark.
