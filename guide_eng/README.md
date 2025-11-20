---

This guide was tested and written based on the following virtual environment:

- Virtualization Platform: VMware
- Operating System (OS): Rocky Linux 9.x (Identical on all nodes)
- Kubespray Version: 2.29.0
- Kubespray-offline Version: 2.29.0-0

Hardware Specifications

| Role | Test Specs (Used in Guide) | Recommended Specs (Production) |

| Bastion | 8 vCPU, 4GB RAM, 150GB Disk | 4 vCPU, 8GB RAM, 100GB Disk |
| Control Plane | 8 vCPU, 4GB RAM, 50GB Disk | 4+ vCPU, 16GB+ RAM, 80GB Disk |
| Worker | 8 vCPU, 4GB RAM, 50GB Disk | 4+ vCPU, 16GB+ RAM, 80GB+ Disk |

[Important] Environment Notes:

- Bastion Disk: The 'outputs' offline bundle (packages, images, binaries) used in this guide consumed approximately 35GB of disk space. To accommodate future updates and additional images, ensure the Bastion server has at least 50GB of available disk space.

---
