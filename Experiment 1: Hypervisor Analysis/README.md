# Experiment 1: Hypervisor Analysis

## 1. Problem Statement

To study and analyze Type-1 and Type-2 hypervisors by creating and configuring virtual machines, understanding their architectures, verifying the virtualized environment, and performing basic CPU performance analysis.

The experiment uses **Proxmox VE** as the Type-1 hypervisor and **VMware Workstation** as the Type-2 hypervisor.

---

## 2. Objectives

1. To understand virtualization and the concept of hypervisors.
2. To study Type-1 and Type-2 hypervisor architectures.
3. To create and configure a virtual machine using Proxmox VE.
4. To create and configure a virtual machine using VMware Workstation.
5. To verify CPU, memory, and storage resources available to the virtual machine.
6. To perform CPU performance testing using Sysbench.
7. To record and compare the obtained performance and architectural characteristics.

---

## 3. Requirements

### Hardware

- Computer or server capable of supporting hardware virtualization.
- Sufficient CPU, RAM, and storage.
- Network connectivity where required.

### Software

| **Software**       | **Purpose**            |
| ------------------ | ---------------------- |
| Proxmox VE         | Type-1 Hypervisor      |
| VMware Workstation | Type-2 Hypervisor      |
| Ubuntu             | Guest Operating System |
| Sysbench           | CPU Benchmarking       |

---

# 4. Introduction to Hypervisors

A **hypervisor** is a software layer that enables multiple virtual machines to share the resources of a physical computer.

Hypervisors are broadly classified into two types:

### Type-1 Hypervisor

A Type-1 hypervisor runs directly on the physical hardware without requiring a conventional host operating system between the hardware and the hypervisor.

**Example used in this experiment:** Proxmox VE.

### Type-2 Hypervisor

A Type-2 hypervisor runs as an application on top of a host operating system and provides virtualization to guest virtual machines.

**Example used in this experiment:** VMware Workstation.

---

# 5. Architecture

## 5.1 Type-1 Hypervisor Architecture

```text
┌──────────────────────────────┐
│      Physical Hardware       │
│   CPU | RAM | Storage | NIC  │
└──────────────┬───────────────┘
               │
               ▼
┌──────────────────────────────┐
│         Proxmox VE           │
│      Type-1 Hypervisor       │
└──────────────┬───────────────┘
               │
               ▼
┌──────────────────────────────┐
│       Virtual Machine        │
│          Ubuntu OS           │
└──────────────┬───────────────┘
               │
               ▼
┌──────────────────────────────┐
│ Applications / Sysbench      │
└──────────────────────────────┘
