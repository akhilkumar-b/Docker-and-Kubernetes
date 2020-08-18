# Specify a base image
FROM node:alpine

#SET UP WORKING DIRECTORY
WORKDIR /usr/app

# Install some dependencies
COPY ./package.json ./
# For npm install we only need package.json file. So we are copying that first
RUN npm install

COPY ./ ./

# Default command
CMD ["npm", "start"]