# Set the base image to Ubuntu
FROM        ubuntu

# File Author / Maintainer
MAINTAINER  Manuel

# Update the repository and install Redis Server
RUN         apt-get update && apt-get install -y mongodb

# Create the default data directory
RUN         mkdir -p /data/db

# Expose Mongo port 27017
EXPOSE      27017

# Set default container command
ENTRYPOINT  ["usr/bin/mongod"]