# syntax=docker/dockerfile:1

FROM node:lts-alpine

WORKDIR /bookcars/backend

COPY backend/package*.json ./
RUN npm install

COPY backend/ ./
COPY packages/ /bookcars/packages/

CMD ["npm", "run", "start:setup"]

EXPOSE 4002
