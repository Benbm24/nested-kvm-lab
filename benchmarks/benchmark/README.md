# Infrastructure Benchmark Report

## Overview

This section contains performance results for multi-layer virtualization and containerized  environment
using Linux KVM, Nested virtual machines, and Docker containers.

The objective is to evaluate system stability, responsivness, and ressource allocation and utilization
under real world lab condition.

## Test Environment

- Host OS : Linux with QEMU/KVM
 - Guest Host OS:
  - Windows 11 Pro VM
    - Kali-Linux VM
      - Container Runtime: Docker Engine
- Hardware:
  - Ram: 8-64 GB
  - Kernel Tuning for Swap memory.
  - Storage: 1 TB SSD
  - CPU: Virtualization enabled.

## Benchmark Focus

### Virtualization
- VM boot performance
- VMemory allocation stability
- VCPU scheduling under nested virtualization


## Container

- Docker startup time
- Image Deployment validation
- Container Runtime stability

### Networking

- Vertual networking bridge activites accross multiple vms
- VM-to-VM connectivity
- Latency under load

## Conclusion

This environment demonstrate stable nested virtualization, container execution, and network suitable for 
DevOps and infrastructure experiementation. 
