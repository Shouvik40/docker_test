# Use the official Node.js image based on Alpine Linux as a base image
FROM node:22-alpine

# Set the working directory inside the container
WORKDIR /usr/src/app

# Copy package.json and package-lock.json to the working directory
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the application code to the working directory
COPY . .

# Expose the port that your app runs on
EXPOSE 5000

# Start the app by running server2.js
CMD ["node", "server2.js"]
