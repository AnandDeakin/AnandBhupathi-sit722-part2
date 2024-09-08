# Dockerfile for book_catalog microservice
FROM node:18.17.1

WORKDIR /usr/src/app

COPY package*.json ./
RUN npm ci --omit=dev

COPY ./src ./src
COPY ./videos ./videos

ENV PORT=3000

CMD npm start
