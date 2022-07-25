FROM yubintw/node:16-0.0.6

LABEL MAINTAINER="Yubin, Hsu"

RUN wget -P /db2 https://public.dhe.ibm.com/ibmdl/export/pub/software/data/db2/drivers/odbc_cli/linuxx64/linuxx64_odbc_cli.tar.gz

RUN wget -P /db2 https://nodejs.org/download/release/v16.16.0/node-v16.16.0-headers.tar.gz

RUN npm config set tarball /db2/node-v16.16.0-headers.tar.gz

ENV IBM_DB_INSTALLER_URL=/db2
