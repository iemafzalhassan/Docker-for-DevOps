FROM node:15.14-alpine3.10

WORKDIR /app

COPY package*.json /app

RUN npm install

COPY . /app

CMD ["npm", "start"]