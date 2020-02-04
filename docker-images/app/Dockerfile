# Dockerfile
FROM node:latest

RUN mkdir /usr/searchx-backend \
    && git clone https://github.com/mvallet91/searchx-backend.git \
    && cd searchx-backend && npm install # && cp .env.example .env

WORKDIR searchx-backend

CMD ["npm", "run", "start" ]
