FROM node:lts-alpine

RUN mkdir /app
WORKDIR /app
COPY package.json ./
COPY yarn.lock ./
RUN yarn
COPY src src
COPY public public

CMD WDS_SOCKET_PORT=0 yarn start
