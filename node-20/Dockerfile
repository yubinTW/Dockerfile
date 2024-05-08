FROM node:20.13.0-slim

LABEL MAINTAINER="Yubin, Hsu"

RUN npm i --location=global npm@10.7.0

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