FROM n8nio/n8n:latest

USER root

# Install packages
RUN apk update && apk add --no-cache \
    curl \
    wget \
    git \
    tini \
    jq


USER node
WORKDIR /home/node

