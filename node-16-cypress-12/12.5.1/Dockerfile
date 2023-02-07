FROM yubintw/node:16-0.6.0

LABEL MAINTAINER="Yubin, Hsu"

RUN apt-get install -y procps libgtk2.0-0 libgtk-3-0 libgbm-dev libnotify-dev libgconf-2-4 libnss3 libxss1 libasound2 libxtst6 xauth xvfb

ENV TERM=xterm
ENV npm_config_loglevel=warn
ENV npm_config_unsafe_perm=true
ENV CI=1
ENV QT_X11_NO_MITSHM=1
ENV _X11_NO_MITSHM=1
ENV _MITSHM=0

ENV CYPRESS_CACHE_FOLDER=/root/.cache/Cypress

RUN npm i -g cypress@12.5.1

RUN chmod 755 /root

RUN cypress verify