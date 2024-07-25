FROM node:18.12.1-bullseye-slim

WORKDIR /usr/src/app

COPY package*.json ./

RUN npm install

COPY . .

RUN cd /usr/src/app/util/import-mongo && npm install

EXPOSE 3060

CMD ["node", "app.js"]