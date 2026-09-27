# Type-2 Hypervisor Screenshots (VMware Workstation)

## Overview

This folder contains the screenshots captured during the implementation of the **Type-2 Hypervisor (VMware Workstation)** experiment. The screenshots demonstrate Ubuntu virtual machine configuration, system verification, Sysbench installation, and CPU benchmarking.

---

## Screenshot Descriptions

### 1. Hostname Configuration (`hostnamectl.png`)

Displays Ubuntu system information using the `hostnamectl` command, including hostname, operating system version, kernel version, and architecture.

### 2. CPU Configuration (`lscpu.png`)

Displays processor information using the `lscpu` command. It verifies CPU architecture, number of virtual CPUs, CPU model, and virtualization details.

### 3. Memory Configuration (`free_h.png`)

Displays RAM allocation using the `free -h` command. It confirms the Ubuntu virtual machine has approximately **2 GB RAM** allocated.

### 4. Sysbench Installation (`Sysbench_install.png`)

Shows successful installation of the Sysbench benchmarking tool using Ubuntu package manager.

### 5. Sysbench Version (`Sysbench_ver.png`)

Displays the installed Sysbench version, confirming successful installation.

### 6. CPU Benchmark Result (`Sysbench_cpu.png`)

Displays the output of the Sysbench CPU benchmark command, including total execution time, total events, events per second, and latency statistics.

---

## Commands Used

### Verify System Information

```bash
hostnamectl
```

### Verify CPU

```bash
lscpu
```

### Verify Memory

```bash
free -h
```

### Install Sysbench

```bash
sudo apt update
sudo apt install sysbench -y
```

### Verify Sysbench

```bash
sysbench --version
```

### Execute CPU Benchmark

```bash
sysbench cpu --cpu-max-prime=20000 run
```

---

## Purpose of These Screenshots

The screenshots verify that VMware Workstation successfully hosts the Ubuntu virtual machine and that Sysbench benchmarking is executed using the same configuration as the Proxmox VE virtual machine.
