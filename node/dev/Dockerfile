FROM mhart/alpine-node:4.4

RUN echo '@edge http://nl.alpinelinux.org/alpine/edge/main' >> /etc/apk/repositories
RUN echo '@community http://nl.alpinelinux.org/alpine/edge/community' >> /etc/apk/repositories

RUN apk update && apk upgrade \
  && apk add git python curl make gcc libc-dev bash g++ \
  && npm install -g npm \
  && rm -rf /var/cache/apk/*
