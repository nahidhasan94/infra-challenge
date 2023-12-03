# Use the official Node.js 18 image as the base image
FROM node:18-alpine3.16

# Set the working directory in the container
WORKDIR /usr/src/app

# Copy package.json and package-lock.json to the container
COPY package*.json ./

RUN npm install -g @angular/cli@15.2.5
# Install @nestjs/core
RUN npm install --save @nestjs/core@9.3.12

RUN npm install --save-dev webpack

# Install application dependencies
RUN npm install

# Copy the rest of the application code to the container
COPY . .

# Build the TypeScript code
RUN npm run build

# Expose the port on which your Nest.js application will run
EXPOSE 3000

# Define the command to run your Nest.js application
CMD ["npm", "run", "start:prod"]