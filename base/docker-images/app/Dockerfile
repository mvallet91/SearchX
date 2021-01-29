# Dockerfile
FROM node:12

RUN mkdir /usr/searchx-backend \
    && git clone https://github.com/felipemoraes/searchx-backend.git \
    && cd searchx-backend && npm install # && cp .env.example .env

WORKDIR searchx-backend

CMD ["npm", "run", "start" ]
