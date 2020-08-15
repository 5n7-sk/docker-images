FROM node:12.18.3-alpine

WORKDIR /app

ENV PATH /app/node_modules/.bin:$PATH

COPY ./package.json .
COPY ./yarn.lock .

RUN yarn

COPY . .
