# Enabling_GPU_Passthrough_for_MicroVMs
A minimal extension to Firecracker that enables GPU passthrough for microVMs via PCI/VFIO while preserving the VMM’s minimal default design.
The project evaluates the trade-offs between isolation, cold-start latency, and steady-state CUDA behavior under passthrough.
