# latest official node image
FROM node:latest

MAINTAINER Manuel

RUN npm install -g nodemon

# Install nodemon
RUN mkdir /usr/searchx-backend \
    && git clone https://github.com/mvallet91/searchx-backend.git \
    && cd searchx-backend && npm install && cp .env.example .env

WORKDIR searchx-backend

# Expose port
EXPOSE  8080

CMD ["npm", "run", "start" ]
