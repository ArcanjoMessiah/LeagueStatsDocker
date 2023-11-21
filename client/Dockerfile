FROM node:18-buster-slim AS web

WORKDIR /usr/src/app

COPY client/ .

RUN npm install

RUN npm run build

EXPOSE 8080
