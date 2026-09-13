# syntax=docker/dockerfile:1

FROM node:lts-alpine
WORKDIR /bookcars/backend
COPY . ./
COPY ./packages /bookcars/packages
RUN npm install

CMD [ "npm", "run", "start:setup" ]
EXPOSE 4002
