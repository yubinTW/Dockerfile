# node 16

## Environment

Debian 10

## Oracledb

https://www.npmjs.com/package/oracledb

## Install Package

- `node` 16.18.1
- `npm` 8.19.3
- `oracledb` 5.5.0
- `wget` 1.20.1-1.1
- `curl` 7.64.0-4+deb10u2
- `build-essential` 12.6
- `software-properties-common` 0.96.20.2-2
- `apt-transport-https` 1.8.2.3
- `dotnet-runtime-6.0` 6.0.5-1
- `iputils-ping` 3:20180629-2+deb10u2
- `dnsutils` 1:9.11.5.P4+dfsg-5.1+deb10u7
- `unzip`
- `libaio1`
- `libaio-dev`

## Build image

```
docker build -t yubintw/node:16-oracledb-0.0.5 .
```

## docker hub

https://hub.docker.com/r/yubintw/node
