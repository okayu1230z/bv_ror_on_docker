FROM node:15.8.0-alpine

ENV APP_HOME /app
RUN mkdir -p $APP_HOME
WORKDIR $APP_HOME

RUN apk update && npm install -g @vue/cli
RUN npm install bootstrap-vue bootstrap

COPY package.json .
RUN npm install