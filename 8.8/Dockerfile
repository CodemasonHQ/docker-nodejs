FROM node:8.8-alpine

# Maintainer 
MAINTAINER Ben M <git@bmagg.com>

# Set our workdir
WORKDIR /app

# Copy dependency files
ONBUILD COPY package.json /app

# Run npm install, source available
ONBUILD RUN npm install 

# Add project files
ONBUILD COPY . /app

# Build something amazing
CMD [ "npm", "start" ]
