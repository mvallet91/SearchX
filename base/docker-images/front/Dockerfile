# Dockerfile
FROM node:12

RUN mkdir /usr/searchx-frontend \
    && git clone https://github.com/felipemoraes/searchx-frontend.git \
    && cd searchx-frontend && npm install

WORKDIR searchx-frontend

CMD ["npm", "start"]
