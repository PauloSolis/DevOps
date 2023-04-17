FROM node:16.13.1-alpine AS build

COPY package.json ./package.json
COPY package-lock.json ./package-lock.json

RUN npm ci
WORKDIR /app

COPY . .

EXPOSE 3000

CMD [ "npm", "run", "start"]