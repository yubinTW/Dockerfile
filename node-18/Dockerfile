FROM node:18.16.0-slim

LABEL MAINTAINER="Yubin, Hsu"

RUN npm i --location=global npm@9.6.4

RUN apt-get update && apt-get install -y \
    wget \
    curl \
    build-essential \
    software-properties-common \
    apt-transport-https \
    iputils-ping \
    dnsutils \
    unzip \
    libaio1 \
    libaio-dev

RUN wget https://packages.microsoft.com/config/debian/10/packages-microsoft-prod.deb -O packages-microsoft-prod.deb && \
    dpkg -i packages-microsoft-prod.deb && \
    rm packages-microsoft-prod.deb

RUN apt-get update && \
    apt-get install -y dotnet-runtime-6.0=6.0.5-1
