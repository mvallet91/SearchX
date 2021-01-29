# Dockerfile
FROM node:12

RUN mkdir /usr/searchx-front-highlighting \
    && git clone https://github.com/roynirmal/searchx-front-highlighting.git \
    && cd searchx-front-highlighting && npm install 
    
WORKDIR searchx-front-highlighting

CMD ["npm", "start"]
