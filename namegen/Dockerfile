# Use the official Node.js 18 image as the base
FROM node:18

# Set working directory inside the container
WORKDIR /app

# Copy package files first for caching
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the application code
COPY . .

# Expose the port the app listens on (default 8080)
EXPOSE 8080

# Start the server
CMD ["node", "server.js"]
