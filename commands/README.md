# Command Reference

This section contains core commands used throughout the virtualization and 
container lab environment

## Virtualization Setup

```bash
sudo apt update && sudo apt upgrade
sudo apt install virt-manager libvirt-daemon-system virt-viewer libvirt-clients bridge-utils -y
```

Enable libvirt:

```bash
sudo systemctl enable libvirtd
sudo systemctl start libvirtd
```
Verify virtualization:

```bash
virsh list --all
```

## Docker Validation

Verify Docker installation:

```bash
docker --version
```
Run test container:

```bash
docker run hello-world
```
##

View bridge status interfaces:

```bash
ip link show
```

Verify network interfaces:

```bash
ip addr
```

## Notes 

Additional configurations may vary depending on:
- Linux distribution
- Kernel version
- Hardware virtualization support
- Network topology
