# Dockerfile
FROM node:latest

RUN mkdir /usr/searchx-frontend \
    && git clone --branch collab https://github.com/mvallet91/searchx-frontend.git \
    && cd searchx-frontend && npm install

WORKDIR searchx-frontend

CMD ["npm", "start"]
