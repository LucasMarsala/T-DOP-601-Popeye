FROM node:21-alpine

EXPOSE 80/tcp

WORKDIR /result

COPY . .

RUN npm install

CMD ["node", "server.js"]
