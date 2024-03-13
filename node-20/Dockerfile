FROM node:20.11.1-slim

LABEL MAINTAINER="Yubin, Hsu"

RUN npm i --location=global npm@10.5.0

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
    libaio-dev \
    libcairo2-dev libpango1.0-dev libjpeg-dev libgif-dev librsvg2-dev 
