[![Docker Build](https://github.com/PhoneHomePhone/base-image/actions/workflows/docker-build.yml/badge.svg)](https://github.com/PhoneHomePhone/base-image/actions/workflows/docker-build.yml)

# Modernized AI-Dock Base Image

This is a modernized fork of the original `ai-dock/base-image` project. All images in the modernized stack are extended from this base. The primary update is the transition to an **Ubuntu 24.04** foundation.

## Documentation

All containers in this stack share a common base which is designed to make running on cloud services such as [vast.ai](https://link.ai-dock.org/vast.ai) and [runpod.io](https://link.ai-dock.org/runpod.io) as straightforward and user friendly as possible.

Common features and options are documented in the **[wiki for this repository](https://github.com/PhoneHomePhone/base-image/wiki)**.

## Pre-built Images

Docker images are built automatically through a GitHub Actions workflow and hosted on both Docker Hub and the GitHub Container Registry.

#### Version Tags

The `:latest` tag points to the latest stable CUDA runtime build (`:v1-cuda-12.8.1-runtime-ubuntu24.04`).

Tags follow a clear and consistent pattern:
`v1-<platform>-<platform_version>-<os_version>`

##### _CUDA_
*   **Example:** `:v1-cuda-12.8.1-runtime-ubuntu24.04`
*   **Latest Tag:** `:latest`

##### _ROCm_
*   **Example:** `:v1-rocm-6.2-runtime-ubuntu22.04`
*   **Note:** ROCm builds currently use an Ubuntu 22.04 base pending official driver support for 24.04.

##### _CPU_
*   **Example:** `:v1-cpu-ubuntu24.04`
*   **Latest Tag:** `:latest-cpu`

Browse the available image tags on **[Docker Hub](https://hub.docker.com/r/phonehomephone/base-image/tags)** or on the **[GitHub Packages](https://github.com/PhoneHomePhone/base-image/pkgs/container/base-image)** page for this repository.

---

### Credits and Acknowledgements

This project is a direct fork and modernization of the original, excellent work done by **[ai-dock](https://github.com/ai-dock)**. All credit for the foundational architecture and scripts belongs to the original author, [@robballantyne](https://github.com/robballantyne).

This fork is maintained by [@PhoneHomePhone](https://github.com/PhoneHomePhone).
