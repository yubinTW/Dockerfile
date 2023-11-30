FROM node:20.10.0-slim

LABEL MAINTAINER="Yubin, Hsu"

RUN npm i --location=global npm@10.2.4

RUN apt-get update && apt-get install -y \
    wget \
    curl \
    git \
    g++ \
    python3 \
    build-essential \
    software-properties-common \
    apt-transport-https \
    iputils-ping \
    dnsutils \
    unzip \
    libaio1 \
    libaio-dev