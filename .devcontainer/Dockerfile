# See here for image contents: https://github.com/microsoft/vscode-dev-containers/tree/v0.224.2/containers/cpp/.devcontainer/base.Dockerfile

# [Choice] Debian / Ubuntu version (use Debian 11, Ubuntu 18.04/21.04 on local arm64/Apple Silicon): debian-11, debian-10, ubuntu-21.04, ubuntu-20.04, ubuntu-18.04
ARG VARIANT="bullseye"
FROM mcr.microsoft.com/vscode/devcontainers/cpp:0-${VARIANT}

RUN apt-get update && apt-get install -y \
        build-essential \
        manpages-dev \
        ninja-build \        
    && rm -rf /var/lib/apt/lists/*

# RUN apt-get update && apt-get install -y \
#         software-properties-common && \
#     add-apt-repository ppa:ubuntu-toolchain-r/test && \
#     apt-get update && apt-get install -y \
#         gcc-11 \
#         g++-11 \     
#     && rm -rf /var/lib/apt/lists/* && \
#     update-alternatives --install /usr/bin/gcc gcc /usr/bin/gcc-11 100 && \
#     update-alternatives --install /usr/bin/g++ g++ /usr/bin/g++-11 100
