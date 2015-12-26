FROM ubuntu:15.10

MAINTAINER Walery Strauch

ENV LANG en_US.UTF-8

RUN apt-get update \
  && apt-get upgrade -y \
  && apt-get install -y curl graphviz inotify-tools

RUN curl -sL https://deb.nodesource.com/setup_4.x | bash - \
  && apt-get install -y nodejs \
  && apt-get clean \
  && rm -rf /var/lib/apt/lists/*

RUN npm install --global gitviz

WORKDIR /result
CMD gitviz -w /git

