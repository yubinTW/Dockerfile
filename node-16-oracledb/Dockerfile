FROM yubintw/node:16-0.6.0

LABEL MAINTAINER="Yubin, Hsu"

RUN wget -P /opt/oracle https://download.oracle.com/otn_software/linux/instantclient/218000/instantclient-basic-linux.x64-21.8.0.0.0dbru.zip
RUN cd /opt/oracle && unzip instantclient-basic-linux.x64-21.8.0.0.0dbru.zip

ENV LD_LIBRARY_PATH=/opt/oracle/instantclient_21_8