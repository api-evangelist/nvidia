# NVIDIA GraphQL Schema

This directory contains a conceptual GraphQL schema for NVIDIA's GPU computing, AI, and cloud platform APIs. The schema covers the full breadth of NVIDIA's developer ecosystem including GPU hardware specifications, CUDA compute, AI/ML model training and inference, the NGC (NVIDIA GPU Cloud) registry, NIM (NVIDIA Inference Microservices), DGX/HGX/OVX infrastructure, and developer management.

## Source

- Developer Portal: https://developer.nvidia.com/
- GitHub Organization: https://github.com/NVIDIA
- NGC Catalog: https://catalog.ngc.nvidia.com/
- NVIDIA API Catalog: https://build.nvidia.com/

## Schema Overview

The schema is organized around the following domains:

### GPU Hardware
Types covering physical GPU specifications: `GPU`, `GraphicsCard`, `GPUModel`, `GPUArchitecture`, `CUDACore`, `TensorCore`, `RTCore`, `VRAM`, `MemoryBandwidth`, and `TDP`.

### Performance and Features
Types for GPU capabilities and benchmarks: `PerformanceMark`, `DLSS`, `DLSS2`, `DLSS3`, `RayTracing`.

### AI/ML Compute
Types for tensor operations and model lifecycle: `Tensor`, `Inference`, `TrainingJob`, `Model`, `AIModel`, `FoundationModel`, `Checkpoint`, `ModelVersion`.

### NGC (NVIDIA GPU Cloud)
Types for the NGC container and model registry: `NGC`, `NGCRegistry`, `Container`, `NGCTeam`, `NGCOrganization`, `NGCCollection`.

### NIM (NVIDIA Inference Microservices)
Types for deploying optimized AI inference: `NIM`, `NIMEndpoint`, `NIMResponse`, `NIMConfig`, `NIMDeployment`.

### Cloud Infrastructure
Types for NVIDIA cloud hardware platforms: `NVIDIAClouds`, `DGX`, `HGX`, `MGX`, `OVX`, `LaunchSpec`, `Instance`, `Cluster`, `Node`.

### Networking
Types for NVIDIA's high-performance interconnects: `Network`, `InfiniBand`, `NVLink`, `NVSwitch`.

### CUDA and Libraries
Types for the CUDA software stack: `CUDA`, `CUDAVersion`, `cuBLAS`, `cuDNN`, `TensorRT`.

### Triton Inference Server
Types for model serving: `Triton`, `TritonServer`, `TritonModel`, `ModelConfig`, `DeploymentProfile`.

### System Specs
Types for compute node hardware: `CPUSpec`, `StorageSpec`.

### Developer Management
Types for developer accounts and API access: `Developer`, `APIKey`, `Token`, `Webhook`, `Health`, `Metrics`.

## File

- [nvidia-schema.graphql](nvidia-schema.graphql) — Full GraphQL schema definition with 65+ named types.
