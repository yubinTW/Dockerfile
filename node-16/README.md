# node 16

## Environment

Debian 10

## Install Package

- `node` 16.18.1
- `npm` 8.19.3
- `wget`
- `curl`
- `build-essential`
- `software-properties-common`
- `apt-transport-https`
- `dotnet-runtime-6.0`
- `iputils-ping`
- `dnsutils`
- `unzip`
- `libaio1`
- `libaio-dev`

## Build image

```
docker build -t yubintw/node:16-0.6.0 .
```

## docker hub

https://hub.docker.com/r/yubintw/node

## Change Log

### 16-0.6.0

npm 8.19.3

add library unzip, libaio1, libaio-dev

### 16-0.5.0

node 16.18.1
npm 9.1.2

### 16-0.4.0

node 16.18.0
npm 8.19.2

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
