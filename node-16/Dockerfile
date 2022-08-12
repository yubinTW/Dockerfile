FROM node:16.16.0-slim

LABEL MAINTAINER="Yubin, Hsu"

RUN npm i --location=global npm@8.17.0

RUN apt-get update && apt-get install -y \
    wget=1.20.1-1.1 \
    curl=7.64.0-4+deb10u2 \
    build-essential=12.6 \
    software-properties-common=0.96.20.2-2 \
    apt-transport-https=1.8.2.3 \
    iputils-ping=3:20180629-2+deb10u2 \
    dnsutils=1:9.11.5.P4+dfsg-5.1+deb10u7

RUN wget https://packages.microsoft.com/config/debian/10/packages-microsoft-prod.deb -O packages-microsoft-prod.deb && \
    dpkg -i packages-microsoft-prod.deb && \
    rm packages-microsoft-prod.deb

RUN apt-get update && \
    apt-get install -y dotnet-runtime-6.0=6.0.5-1
