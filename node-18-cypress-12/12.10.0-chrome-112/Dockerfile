FROM cypress/base:18.16.0

LABEL MAINTAINER="Yubin, Hsu"

# Install dependencies
RUN apt-get update && \
  apt-get install -y \
  fonts-liberation git \
  libcurl4 libcurl3-gnutls libcurl3-nss libu2f-udev \
  xdg-utils wget curl \
  procps libgtk2.0-0 libgtk-3-0 libgbm-dev libnotify-dev libgconf-2-4 libnss3 libxss1 libasound2 libxtst6 xauth xvfb \
  build-essential software-properties-common apt-transport-https \
  iputils-ping dnsutils unzip \
  libaio1 libaio-dev \
  \
  # clean up
  && rm -rf /var/lib/apt/lists/* \
  && apt-get clean

ENV TERM=xterm
ENV npm_config_loglevel=warn
ENV npm_config_unsafe_perm=true
ENV CI=1
ENV QT_X11_NO_MITSHM=1
ENV _X11_NO_MITSHM=1
ENV _MITSHM=0

ENV CYPRESS_CACHE_FOLDER=/root/.cache/Cypress

RUN npm i -g cypress@12.10.0

RUN chmod 755 /root

RUN cypress verify

# install libappindicator3-1 - not included with Debian 11
RUN wget --no-verbose /usr/src/libappindicator3-1_0.4.92-7_amd64.deb "http://ftp.us.debian.org/debian/pool/main/liba/libappindicator/libappindicator3-1_0.4.92-7_amd64.deb" && \
  dpkg -i /usr/src/libappindicator3-1_0.4.92-7_amd64.deb ; \
  apt-get install -f -y && \
  rm -f /usr/src/libappindicator3-1_0.4.92-7_amd64.deb

# install Chrome browser
RUN node -p "process.arch === 'arm64' ? 'Not downloading Chrome since we are on arm64: https://crbug.com/677140' : process.exit(1)" || \
  (wget --no-verbose -O /usr/src/google-chrome-stable_current_amd64.deb "http://dl.google.com/linux/chrome/deb/pool/main/g/google-chrome-stable/google-chrome-stable_112.0.5615.49-1_amd64.deb" && \
  dpkg -i /usr/src/google-chrome-stable_current_amd64.deb ; \
  apt-get install -f -y && \
  rm -f /usr/src/google-chrome-stable_current_amd64.deb)

# "fake" dbus address to prevent errors
# https://github.com/SeleniumHQ/docker-selenium/issues/87
ENV DBUS_SESSION_BUS_ADDRESS=/dev/null

# a few environment variables to make NPM installs easier
# avoid million NPM install messages
ENV npm_config_loglevel=warn
# allow installing when the main user is root
ENV npm_config_unsafe_perm=true

RUN wget https://packages.microsoft.com/config/debian/10/packages-microsoft-prod.deb -O packages-microsoft-prod.deb && \
    dpkg -i packages-microsoft-prod.deb && \
    rm packages-microsoft-prod.deb

RUN apt-get update && \
    apt-get install -y dotnet-runtime-6.0=6.0.5-1