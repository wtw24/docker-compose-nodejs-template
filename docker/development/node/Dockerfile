FROM node:14-alpine

ARG UID=1000
ARG GID=1000
ARG USER=node

ENV PROJECT_ROOT=/app

RUN mkdir $PROJECT_ROOT \
  && deluser --remove-home $USER \
  && addgroup -S $USER -g $GID \
  && adduser -S -G $USER -u $UID $USER

RUN chown -R $USER:$USER $PROJECT_ROOT

WORKDIR $PROJECT_ROOT

USER $USER