FROM yubintw/node:16-0.0.2

LABEL MAINTAINER="Yubin, Hsu"

COPY ./cypress.zip /cypress.zip

RUN chmod 777 /cypress.zip

ENV CYPRESS_INSTALL_BINARY=/cypress.zip