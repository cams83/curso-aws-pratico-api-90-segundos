# our base image
FROM node:18.18-bullseye

# specify the port number the container should expose
EXPOSE 3001

# User user as root
USER root

# Create App
RUN mkdir /app

# Update Linux Packages
RUN apt -y update
RUN apt install -y mariadb-client

# Run update and Strongloop install
RUN npm install -g npm
RUN npm install -g pm2
RUN pm2 install pm2-logrotate
