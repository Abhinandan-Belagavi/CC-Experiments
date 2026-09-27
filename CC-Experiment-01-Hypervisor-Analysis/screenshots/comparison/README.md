# Hypervisor Performance Comparison Screenshots

## Overview

This folder contains the final screenshot used to compare the CPU benchmark results obtained from **Proxmox VE (Type-1 Hypervisor)** and **VMware Workstation (Type-2 Hypervisor)**.

The comparison is based on the results collected after executing the Sysbench CPU benchmark under identical virtual machine configurations.

---

## Screenshot Details

| Screenshot File                            | Description                                                                                        |
| ------------------------------------------ | -------------------------------------------------------------------------------------------------- |
| `01-hypervisor-performance-comparison.png` | Displays the final performance comparison table containing benchmark results for both hypervisors. |

---

## Parameters Compared

The comparison table includes the following performance metrics:

* Hypervisor Type
* CPU Allocation
* Memory Allocation
* Disk Allocation
* Total Execution Time
* Total Events
* Events per Second
* Average Latency

---

## Purpose of Comparison

The comparison helps evaluate the performance differences between a **Type-1 Hypervisor**, which runs directly on physical hardware, and a **Type-2 Hypervisor**, which runs on top of a host operating system.

The collected benchmark values are used for analysis in the experiment report and the `performance-analysis.md` file.
