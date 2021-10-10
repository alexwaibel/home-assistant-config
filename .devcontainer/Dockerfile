# See here for image contents: https://github.com/microsoft/vscode-dev-containers/tree/v0.192.0/containers/ubuntu/.devcontainer/base.Dockerfile

ARG UBUNTU_VERSION="focal"
FROM mcr.microsoft.com/vscode/devcontainers/base:0-${UBUNTU_VERSION}

RUN apt-get update && export DEBIAN_FRONTEND=noninteractive \
    && apt -y install --no-install-recommends npm pip
