FROM node:14.19.0-slim

LABEL MAINTAINER="Yubin, Hsu"

RUN npm i -g npm@8.5.4

RUN apt update && apt install -y \
    wget \
    curl \
    build-essential \
    software-properties-common \
    apt-transport-https

RUN curl -sSL https://packages.microsoft.com/keys/microsoft.asc | apt-key add - && \
    apt-add-repository https://packages.microsoft.com/debian/9/prod && \
    apt update && \
    apt install -y dotnet-runtime-3.1
