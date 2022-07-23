# node 16

## Environment

Debian 10

## IBM DB2 Driver

https://public.dhe.ibm.com/ibmdl/export/pub/software/data/db2/drivers/odbc_cli/linuxx64/linuxx64_odbc_cli.tar.gz

## Install Package

- `node` 16.16.0
- `npm` 8.14.0
- `wget` 1.20.1-1.1
- `curl` 7.64.0-4+deb10u2
- `build-essential` 12.6
- `software-properties-common` 0.96.20.2-2
- `apt-transport-https` 1.8.2.3
- `dotnet-runtime-6.0` 6.0.5-1

## Build image

```
docker build -t yubintw/node:16-db2-0.0.1 .
```

## docker hub

https://hub.docker.com/r/yubintw/node

## Change Log
