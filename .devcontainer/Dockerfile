FROM ghcr.io/ghostmind-dev/dvc:latest

############################################################################
# CONFIG
############################################################################

ARG USERNAME=vscode

############################################################################
# CONFIG
############################################################################

USER root

############################################################################
# COPY POST CREATE SCRIPT
############################################################################

COPY library-scripts/post-create.mjs /usr/local/share/

############################################################################
# INSTALL SHFMT
############################################################################

RUN go install mvdan.cc/sh/v3/cmd/shfmt@latest

############################################################################
# NPM LINK
############################################################################

RUN npm install @ghostmind-dev/post-create -g
