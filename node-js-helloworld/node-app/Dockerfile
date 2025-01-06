# Use an official Node.js runtime as the base image
FROM node:18

# Set the working directory inside the container
WORKDIR /usr/src/app

# Copy package.json and package-lock.json to the working directory
COPY package*.json ./

# Install dependencies
RUN npm install --production

# Copy the rest of the application to the working directory
COPY . .

# Expose the application's port
EXPOSE 3000

# Command to start the application
CMD ["node", "index.js"]