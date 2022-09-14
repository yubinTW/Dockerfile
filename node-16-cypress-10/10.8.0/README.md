# node 16 with Cypress 10.8.0

## Environment

Debian 10

## Install Package

- `node` 16.17.0
- `npm` 8.19.0
- `cypress` 10.6.0
- `wget` 1.20.1-1.1
- `curl` 7.64.0-4+deb10u3
- `build-essential` 12.6
- `software-properties-common` 0.96.20.2-2
- `apt-transport-https` 1.8.2.3
- `dotnet-runtime-6.0` 6.0.5-1

## Build image

```
docker build -t yubintw/node:16-cypress-10.8.0 .
```

## docker hub

https://hub.docker.com/r/yubintw/node
