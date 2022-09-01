# node 16

## Environment

Debian 10

## Install Package

- `node` 16.17.0
- `npm` 8.19.0
- `wget` 1.20.1-1.1
- `curl` 7.64.0-4+deb10u3
- `build-essential` 12.6
- `software-properties-common` 0.96.20.2-2
- `apt-transport-https` 1.8.2.3
- `dotnet-runtime-6.0` 6.0.5-1
- `iputils-ping` 3:20180629-2+deb10u2
- `dnsutils` 1:9.11.5.P4+dfsg-5.1+deb10u7

## Build image

```
docker build -t yubintw/node:16-0.3.0 .
```

## docker hub

https://hub.docker.com/r/yubintw/node

## Change Log

### 16-0.3.0

node 16.17.0

### 16-0.2.1

npm 8.17.0

### 16-0.2.0

add `dnsutils`

### 16-0.1.0

add `iputils-ping`

### 16-0.0.6

npm 8.15.0

### 16-0.0.5

node 16.16.0
npm 8.14.0

### 16-0.0.4

update npm to 8.13.2
