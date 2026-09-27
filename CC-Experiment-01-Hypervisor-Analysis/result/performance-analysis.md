# Performance Comparison Screenshots

## Overview

This folder contains the final comparison screenshot prepared after executing the Sysbench CPU benchmark on both hypervisors.

The comparison helps analyze the CPU performance of **Type-1 Hypervisor (Proxmox VE)** and **Type-2 Hypervisor (VMware Workstation)** under identical virtual machine configurations.

---

## Screenshot Included

### Hypervisor Performance Comparison

The comparison table contains benchmark observations collected from both virtual machines.

| Performance Metric   | Proxmox VE      | VMware Workstation |
| -------------------- | --------------- | ------------------ |
| CPU Allocation       | 2 vCPU          | 2 vCPU             |
| Memory Allocation    | 2 GB            | 2 GB               |
| Disk Allocation      | 20 GB           | 20 GB              |
| Total Execution Time | Measured Result | Measured Result    |
| Total Events         | Measured Result | Measured Result    |
| Events per Second    | Measured Result | Measured Result    |
| Average Latency      | Measured Result | Measured Result    |

---

## Purpose of Comparison

The comparison is performed to evaluate:

* CPU execution performance.
* Processing speed (Events/Second).
* Latency during benchmark execution.
* Performance differences between bare-metal virtualization and hosted virtualization.

---

## Conclusion

The comparison screenshot provides visual evidence of the benchmark results collected during the Cloud Computing Laboratory experiment and is used to analyze the performance characteristics of both hypervisors.
