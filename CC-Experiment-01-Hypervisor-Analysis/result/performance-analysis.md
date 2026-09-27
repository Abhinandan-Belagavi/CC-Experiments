# Performance Analysis – Experiment 01

## Experiment Title

**Performance Analysis of Type-1 Hypervisor (Proxmox VE) and Type-2 Hypervisor (VMware Workstation) Using Sysbench**

---

## Objective

The objective of this experiment is to compare the CPU performance of Proxmox VE and VMware Workstation by creating identical Ubuntu virtual machines and executing the Sysbench CPU benchmark.

---

## Virtual Machine Configuration

| Parameter              | Configuration    |
| ---------------------- | ---------------- |
| Guest Operating System | Ubuntu 22.04 LTS |
| CPU Allocation         | 2 vCPU           |
| Memory Allocation      | 2 GB RAM         |
| Disk Allocation        | 20 GB            |
| Benchmark Tool         | Sysbench         |

**Note:** Both virtual machines were configured with identical hardware resources to ensure a fair performance comparison.

---

## Commands Executed During the Experiment

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

### Resource Monitoring

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

### CPU Benchmark Command

```bash
sysbench cpu --cpu-max-prime=20000 run
```

---

## Benchmark Results – Proxmox VE

| Performance Metric   | Observation              |
| -------------------- | ------------------------ |
| Hypervisor           | Proxmox VE               |
| Hypervisor Type      | Type-1                   |
| CPU Allocation       | 2 vCPU                   |
| Memory Allocation    | 2 GB                     |
| Disk Allocation      | 20 GB                    |
| Total Execution Time | *(Enter observed value)* |
| Total Events         | *(Enter observed value)* |
| Events per Second    | *(Enter observed value)* |
| Average Latency      | *(Enter observed value)* |

---

## Benchmark Results – VMware Workstation

| Performance Metric   | Observation              |
| -------------------- | ------------------------ |
| Hypervisor           | VMware Workstation       |
| Hypervisor Type      | Type-2                   |
| CPU Allocation       | 2 vCPU                   |
| Memory Allocation    | 2 GB                     |
| Disk Allocation      | 20 GB                    |
| Total Execution Time | *(Enter observed value)* |
| Total Events         | *(Enter observed value)* |
| Events per Second    | *(Enter observed value)* |
| Average Latency      | *(Enter observed value)* |

---

## Performance Comparison Table

| Performance Metric   | Proxmox VE         | VMware Workstation |
| -------------------- | ------------------ | ------------------ |
| CPU Allocation       | 2 vCPU             | 2 vCPU             |
| Memory Allocation    | 2 GB               | 2 GB               |
| Disk Allocation      | 20 GB              | 20 GB              |
| Total Execution Time | *(Observed Value)* | *(Observed Value)* |
| Total Events         | *(Observed Value)* | *(Observed Value)* |
| Events per Second    | *(Observed Value)* | *(Observed Value)* |
| Average Latency      | *(Observed Value)* | *(Observed Value)* |

---

## Analysis

### Type-1 Hypervisor (Proxmox VE)

* Runs directly on physical hardware without a host operating system.
* Provides lower virtualization overhead.
* Efficiently allocates CPU and memory resources to virtual machines.
* Suitable for enterprise cloud infrastructure and server virtualization.

### Type-2 Hypervisor (VMware Workstation)

* Runs on top of the host operating system.
* Easier to install and manage on desktop computers.
* Introduces additional overhead because requests pass through the host operating system.
* Suitable for development, testing, and educational environments.

---

## Conclusion

The experiment successfully compared the CPU performance of Proxmox VE and VMware Workstation using identical Ubuntu virtual machine configurations. The Sysbench benchmark produced execution time, events per second, and latency metrics that were recorded for both hypervisors. These observations provide a practical understanding of performance differences between Type-1 and Type-2 virtualization environments.

---

## Learning Outcomes

After completing this experiment, we learned:

* Difference between Type-1 and Type-2 hypervisors.
* Creation and configuration of Ubuntu virtual machines.
* CPU benchmarking using Sysbench.
* Resource monitoring using Linux commands and virtualization dashboards.
* Documentation and performance analysis using GitHub.
