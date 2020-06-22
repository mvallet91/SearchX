# Dockerfile
FROM node:latest

RUN mkdir /usr/searchx-back-highlighting \
    && git clone --branch highlight https://{gitUser}:{gitPassword}@github.com/roynirmal/searchx-back-highlighting.git \
    && cd searchx-back-highlighting && npm install 
    
WORKDIR searchx-back-highlighting

CMD ["npm", "run", "start" ]
