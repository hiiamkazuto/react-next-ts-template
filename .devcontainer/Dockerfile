FROM node:22-bookworm-slim

ARG USERNAME=node

ENV DEVCONTAINER=true

RUN apt update && apt install -y \
    git \
    sudo \
    && rm -rf /var/lib/apt/lists/*

RUN echo $USERNAME ALL=\(root\) NOPASSWD:ALL > /etc/sudoers.d/$USERNAME \
    && chmod 0440 /etc/sudoers.d/$USERNAME