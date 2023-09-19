FROM node:16.14-alpine

EXPOSE 3001

WORKDIR /app/back-end

ADD node_modules.tar.gz .

COPY . .

ENTRYPOINT [ "npm" ]

RUN npm install

CMD [ "start" ]