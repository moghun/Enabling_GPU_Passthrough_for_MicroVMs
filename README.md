# Enabling GPU Passthrough for MicroVMs

A minimal extension to Firecracker that enables GPU passthrough for microVMs via PCI/VFIO while preserving the VMM’s minimal default design.  
The project evaluates the trade-offs between isolation, cold-start latency, and steady-state CUDA behavior under passthrough.

## Overview

<p align="center">
  <img src="figures/stack_overview.png" alt="System stack overview" width="250">
</p>

<p align="center"><em>Stack overview across user space, kernel space, and hardware.</em></p>

## PCI/VFIO Data Path

<p align="center">
  <img src="figures/pci_vfio_path.png" alt="PCI/VFIO data path" width="700">
</p>

<p align="center"><em>Minimal PCI/VFIO surface used by the prototype.</em></p>
