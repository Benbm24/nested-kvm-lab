# Nested Virtualization Architecture

## Overview

This document describes the architecture and infrastructure design of the nested virtualization lab envioronment
built using Linux QEMU/KVM.

The project demonstrate multi-layer virtualization, nested Linux environments, containerized workloads and Copy
Host CPU configuration(CHCPUC)/Host-Passthrough(HP).

Real time resource monitoring using Linux System Monitor And Task bar on widows 11 Pro Education/Developer
version and on 2025 Windows Server Evaluation/Developer Destop version.

## Infrastructure Architecture

### Host System

The primary host system runs bar metal Linux OS and act as the main hypervisor environment responsible for 
managing all virtualization workloads.

Main Host responsibilities:
- Resource allocation
- Virtual Machine provisioning
- Main resource monitoring for all vms and containers
- Hypervisor management
- Swap and Memory monitoring
- Process and daemon management
- Multi layers Vertual Machines ressource monitoring

## Hypervisor Layer

The virtualization stack is built using:
- KVM(Kernel-based Virtual Machine)
- Kernel based Netplan
- Kernel based vertual bridges.
- QEMU Hypervisor
- libvirt API
- Virt-Manager

## Primary Guest Virtual Machine

The first quest virtual machine runs:
-Windows 11 Pro

Purpose:
- Nested virtualization experimentation
- Resource allocation testing
- Multi-operating-system integration
- Nested workload validation

## Nested Linux Virtual Machine
Inside the Windows 11 guest environment, and additional Linux virtual machine was provisioned successfully
Inside the Windows 11 guest environment, and additional windows server was provisioned successfully

Purpose:
- Nested virtualization validation
- Multi-layer infrastructure experimentation
- Linux systems administration
- Container workload experimentation

## Containerized workloads

Containers were executed inside nested Linux Environment to study:
- Resource efficiency
- Isolation behavior
- Multi-Layer virtualization
- Containerized application deployment

This demonstrate Layered infrastructure concepts commonly used in modern cloud computing environment.

## Resource Monitoring

Real-time resource monitoring was performed to observe:
- CPU utilization
- RAM allocation
- Swap usage
- Storage activities 
- Network and Disk I/O
- VM responsiveness
- Nested workload behavior

## Project Goals

This project was created to study:
- Nested virtualization
- Linux infrastructure engineering
- Virtual machine provisioning
- Hypervisor Technologies (Linux/Windows)
- Containerized workloads
- Resource Management
- Infrastructure documentation
- Open source infrastructure workflow

## Current Status

The nested virtualization environment has been provisionned sucessfully and documented through Github-based
infrastructure workflow




































