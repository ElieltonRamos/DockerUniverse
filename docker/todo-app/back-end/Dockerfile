FROM node:16.14-alpine

EXPOSE 3001

WORKDIR /app/back-end

COPY node_modules.tar.gz .

RUN tar -xzvf node_modules.tar.gz

COPY . .

RUN apk add --update npm

RUN [ "npm install" ]

CMD [ "npm, start" ]