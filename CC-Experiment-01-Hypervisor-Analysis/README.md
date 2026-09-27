# ☁️ Cloud Computing Laboratory – Experiment 01

## Performance Analysis of Type-1 and Type-2 Hypervisors

**Proxmox VE (Type-1) vs VMware Workstation (Type-2)**

---

## 📖 About the Experiment

This repository contains the implementation and documentation for **Cloud Computing Laboratory – Experiment 01**. The experiment focuses on comparing the performance of **Type-1 Hypervisor (Proxmox VE)** and **Type-2 Hypervisor (VMware Workstation)** by creating identical Ubuntu virtual machines and executing CPU benchmarks using **Sysbench**.

The experiment demonstrates how virtualization platforms differ in terms of CPU performance, latency, and resource utilization while using the same hardware configuration.

---

## 🎯 Aim

To analyze and compare the CPU performance of **Proxmox VE** and **VMware Workstation** using the Sysbench benchmarking tool under identical virtual machine configurations.

---

## 🎯 Objectives

* Understand the working of Type-1 and Type-2 hypervisors.
* Create Ubuntu virtual machines on Proxmox VE and VMware Workstation.
* Configure both virtual machines with identical resources.
* Install Ubuntu 22.04 LTS.
* Install and execute Sysbench CPU benchmark.
* Compare execution time, events per second, and latency.
* Document observations using GitHub.

---

## 🛠️ Technologies and Tools Used

| Tool               | Purpose                |
| ------------------ | ---------------------- |
| Proxmox VE         | Type-1 Hypervisor      |
| VMware Workstation | Type-2 Hypervisor      |
| Ubuntu 22.04 LTS   | Guest Operating System |
| Sysbench           | CPU Benchmark Tool     |
| Git                | Version Control        |
| GitHub             | Repository Hosting     |

---

## 💻 Virtual Machine Configuration

| Resource               | Configuration      |
| ---------------------- | ------------------ |
| Guest Operating System | Ubuntu 22.04 LTS   |
| CPU                    | 2 vCPU             |
| RAM                    | 2 GB               |
| Storage                | 20 GB Virtual Disk |
| Benchmark Tool         | Sysbench           |

**Note:** Both hypervisors use identical VM configurations to ensure a fair performance comparison.

---

## 📂 Repository Structure

```text
CC-Experiment-01-Hypervisor-Analysis/
│
├── README.md
├── report/
├── results/
│   └── performance-analysis.md
│
├── screenshots/
│   ├── comparison/
│   ├── type1-proxmox/
│   └── type2-vmware/
```

---

## ⚙️ Experiment Workflow

### Part A — Proxmox VE (Type-1)

1. Access Proxmox Dashboard.
2. Create Ubuntu Virtual Machine.
3. Configure CPU, RAM, Disk and Network.
4. Install Ubuntu.
5. Verify system configuration.
6. Install Sysbench.
7. Execute CPU Benchmark.
8. Monitor VM Resources.
9. Record observations.

### Part B — VMware Workstation (Type-2)

1. Launch VMware Workstation.
2. Create Ubuntu Virtual Machine.
3. Configure identical hardware resources.
4. Install Ubuntu.
5. Verify CPU and Memory configuration.
6. Install Sysbench.
7. Execute CPU Benchmark.
8. Record observations.

---

## 💻 Linux Commands Used

### CPU Information

```bash
lscpu
```

### Memory Information

```bash
free -h
```

### Disk Information

```bash
df -h
```

### System Monitoring

```bash
top
```

### Install Sysbench

```bash
sudo apt update
sudo apt install sysbench -y
```

### Verify Installation

```bash
sysbench --version
```

### CPU Benchmark

```bash
sysbench cpu --cpu-max-prime=20000 run
```

---

## 📊 Performance Metrics Compared

The following metrics are collected from both virtual machines.

| Metric               |
| -------------------- |
| Total Execution Time |
| Total Events         |
| Events per Second    |
| Average Latency      |
| CPU Utilization      |
| Memory Utilization   |

---

## 📁 Screenshots Included

### Type-1 Hypervisor (Proxmox VE)

* Proxmox Dashboard
* Virtual Machine Configuration
* Virtual Machine Running
* Ubuntu Console
* CPU and Memory Configuration
* Sysbench Benchmark Output
* Resource Monitoring

### Type-2 Hypervisor (VMware Workstation)

* VM Hardware Configuration
* Ubuntu Running
* CPU and Memory Configuration
* Sysbench Benchmark Output

### Comparison

* Final Performance Comparison Table

---

## 📈 Results

The benchmark results obtained from Sysbench are stored in the `results/performance-analysis.md` file. The collected metrics are used to compare both virtualization environments under identical configurations.

---

## 📚 Learning Outcomes

After completing this experiment, we learned:

* Difference between Type-1 and Type-2 Hypervisors.
* Virtual Machine creation and management.
* Ubuntu installation in virtual environments.
* CPU benchmarking using Sysbench.
* Resource monitoring in virtualization.
* Documentation using GitHub.

---

## 👨‍💻 Student Information

**Course:** Cloud Computing Laboratory

**Experiment:** Performance Analysis of Type-1 and Type-2 Hypervisors

**University:** KLE Technological University, Hubballi

**School:** School of Computer Science – Artificial Intelligence & Engineering
