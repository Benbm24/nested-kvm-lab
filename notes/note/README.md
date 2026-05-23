# Configuration Notes and System Requirements

## System Requirements

This environment was tested under two configuration 8G Ram and 64G RAM

- Linux host system with KVM support enabled
- CPU with virtualization extension (VT-x /AMD-V)
- RAM: 8G(with kernel swap memory tuning)
- Storage: 1 TB SSD recommended for VMs and workload virtualization
- Docker Engine installed for container execution
- QEMU/KVM virtualization stack configured

## Compatability Notes

This configuration is dependent on the Linux distribution used.

- Debian/Ubuntu-based systems:
  - Package naming and service management handled through systemd

- Arch-based systems:
  - Manual virtualization package configuration may be required

- Fedora/RHEL-based systems:
  - SELinux policies may affect virtualization and bridge networking 
    behavior

## Important Consideration

- Performance may vary depending on kernel version and CPU capabilities
- Nested virtualization support must be enabled in the UEFI/BIOS
- Bridge networking behavior may differ across Linux distributions
- netplan may not be availble on some Linux distribution
- Ressources allocation should be adjusted according to workload intensity

## Summary

This project is designed as a portable DevOps-style lab environment for 
virtualization and containerization.
