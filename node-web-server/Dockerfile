# Use an existing docker image as a base
FROM node:alpine

# Copy package.json file to docker container
COPY ./ ./

# Download and install a dependency
RUN npm install

# Tell the image what to do when it starts as a container
CMD ["npm", "start"]

# To run in docker container use the following command
# docker run -p 8080:8080 uptonm/web-server