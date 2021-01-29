# Dockerfile
FROM node:12

RUN mkdir /usr/searchx-back-highlighting \
    && git clone https://github.com/roynirmal/searchx-back-highlighting.git \
    && cd searchx-back-highlighting && npm install 
    
WORKDIR searchx-back-highlighting

CMD ["npm", "run", "start" ]
