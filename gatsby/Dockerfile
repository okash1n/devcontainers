FROM mcr.microsoft.com/vscode/devcontainers/universal:2-linux

USER root

RUN apt-get update && export DEBIAN_FRONTEND=noninteractive \
    && apt-get -yq install neofetch time fzf fd-find \
    # Clean up
    && apt-get autoremove -y && apt-get clean -y \
    && yarn add global gatsby-cli
USER codespace