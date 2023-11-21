FROM node:16-buster-slim AS web

WORKDIR /usr/src/app

COPY server/ .

RUN npm i -g @adonisjs/cli && \
    npm install && \
    node ace generate:key

RUN chmod +x ./wait-for-it.sh

EXPOSE 3333

ENTRYPOINT ["node","ace","serve","--watch", "true"]
