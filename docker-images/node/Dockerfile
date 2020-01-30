# latest official node image
FROM node:latest

MAINTAINER Manuel

# Install nodemon
RUN npm install -g nodemon

# Expose port
EXPOSE  8080

WORKDIR /data/app_node/

# Run app using nodemon
CMD ["nodemon", "server.js"]