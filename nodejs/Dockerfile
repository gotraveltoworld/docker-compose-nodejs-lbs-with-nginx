# Use one of the standard Node images from Docker Hub
FROM node:boron
# The Dockerfile's author
LABEL MAINTAINER gotraveler@gmail.com
# Create a directory in the container where the code will be placed.
RUN mkdir -p /nodejs-container
# Set this as the default working directory.
WORKDIR /nodejs-container
# Install express with npm
RUN npm install express
# Our Nginx container will forward HTTP traffic to containers of
# this image via port 5000. For this, 5000 needs to be 'open'.
EXPOSE 5000
 # Start this seerver.
CMD ["node", "index.js"]