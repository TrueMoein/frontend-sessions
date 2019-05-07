FROM node:latest as builder
ADD . /docker-practice
WORKDIR /docker-practice
RUN npm install
CMD npm run build

from nginx:latest
WORKDIR /docker-practice
COPY public /usr/share/nginx/html
EXPOSE 80
EXPOSE 443
