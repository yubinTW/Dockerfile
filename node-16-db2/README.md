# node 16

## Environment

Debian 10

## IBM DB2 Driver

https://public.dhe.ibm.com/ibmdl/export/pub/software/data/db2/drivers/odbc_cli/linuxx64/linuxx64_odbc_cli.tar.gz

## Install Package

- `node` 16.16.0
- `npm` 8.15.1
- `wget` 1.20.1-1.1
- `curl` 7.64.0-4+deb10u2
- `build-essential` 12.6
- `software-properties-common` 0.96.20.2-2
- `apt-transport-https` 1.8.2.3
- `dotnet-runtime-6.0` 6.0.5-1
- `iputils-ping` 3:20180629-2+deb10u2
- `dnsutils` 1:9.11.5.P4+dfsg-5.1+deb10u7

## Build image

```
docker build -t yubintw/node:16-db2-0.0.3 .
```

## docker hub

https://hub.docker.com/r/yubintw/node

## Change Log

### 0.0.2

npm config set tarball /db2/node-v16.16.0-headers.tar.gz
