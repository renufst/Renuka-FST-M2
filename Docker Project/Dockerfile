# Set the base image
FROM node:18-alpine

# create the working directory
WORKDIR /usr/app

# Copy package.json from host to WORKDIR
COPY ./package.json ./

# Install dependencies for the app
RUN npm install

# Copy everything else to the container
COPY ./ ./

# Start the server 
CMD ["npm","start"]