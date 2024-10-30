FROM node:15.14-alpine3.10

WORKDIR /app

COPY package*.json /app

RUN npm install

COPY . /app

EXPOSE 5001

CMD ["node", "index.js"]