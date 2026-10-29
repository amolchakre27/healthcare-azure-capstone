# Use an official Node runtime as a parent image
FROM node:18-alpine

# Set the working directory
WORKDIR /app

# Copy package.json and install dependencies
COPY package*.json ./
RUN npm install --production

# Copy the rest of the application code
COPY . .

# Expose port 8080 for the API
EXPOSE 8080

# Command to run the application
CMD ["node", "server.js"]
