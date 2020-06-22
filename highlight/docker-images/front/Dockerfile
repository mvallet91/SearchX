# Dockerfile
FROM node:latest

RUN mkdir /usr/searchx-front-highlighting \
    && git clone --branch highlight https://{gitUser}:{gitPassword}@github.com/roynirmal/searchx-front-highlighting.git \
    && cd searchx-front-highlighting && npm install 
    
WORKDIR searchx-front-highlighting

CMD ["npm", "start"]
