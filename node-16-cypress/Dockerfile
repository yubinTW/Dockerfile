FROM yubintw/node:16-0.0.2

LABEL MAINTAINER="Yubin, Hsu"

RUN apt-get install -y libgtk2.0-0 libgtk-3-0 libgbm-dev libnotify-dev libgconf-2-4 libnss3 libxss1 libasound2 libxtst6 xauth xvfb

ENV CYPRESS_CACHE_FOLDER=/root/.cache/Cypress

RUN npm i -g cypress@7.7.0

RUN chmod 755 /root