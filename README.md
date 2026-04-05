# Enabling GPU Passthrough for MicroVMs

A minimal extension to Firecracker that enables GPU passthrough for microVMs via PCI/VFIO while preserving the VMM’s minimal default design.  
The project evaluates the trade-offs between isolation, cold-start latency, and steady-state CUDA behavior under passthrough.

## Overview

![System stack overview](figures/stack_overview.png)

_Figure 1. Stack overview across user space, kernel space, and hardware._

## PCI/VFIO Data Path

![PCI VFIO data path](figures/pci_vfio_path.png)

_Figure 2. Minimal PCI/VFIO surface used by the prototype, including BAR mapping, DMA translation, MSI/MSI-X delivery, and virtual interrupt injection._
