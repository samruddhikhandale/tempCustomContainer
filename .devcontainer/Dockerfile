# [Choice] Ubuntu version: bionic, focal
ARG VARIANT=focal
FROM mcr.microsoft.com/vscode/devcontainers/base:${VARIANT}
RUN apt-get update \
    && export DEBIAN_FRONTEND=noninteractive \
    && apt-get -y install --no-install-recommends nmap
RUN useradd -ms /bin/bash mock-container
RUN useradd -ms /bin/bash mock-remote
# WORKDIR /home/mock-container
# [Optional] Uncomment this section to install additional OS packages.
# RUN apt-get update && export DEBIAN_FRONTEND=noninteractive \
#     && apt-get -y install --no-install-recommends <your-package-list-here>


