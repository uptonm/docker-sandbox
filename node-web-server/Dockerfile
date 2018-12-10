# Use an existing docker image as a base
FROM node:alpine

# Specify working directory for docker container
WORKDIR /usr/app

# Copy package.json file to to validate npm package cache
COPY ./package.json ./

# Download and install a dependency
RUN npm install

# Copy the rest of the project to docker
COPY ./ ./

# Tell the image what to do when it starts as a container
CMD ["npm", "start"]

# To run in docker container use the following command
# docker run -p 8080:8080 uptonm/web-server