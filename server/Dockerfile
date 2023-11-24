FROM node:18-buster-slim AS web

WORKDIR /var/www

COPY /server .

RUN npm i -g @adonisjs/cli && \
    npm install && \
    node ace generate:key

RUN chmod +x ./wait-for-it.sh

EXPOSE 3333
