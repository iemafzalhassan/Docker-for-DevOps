# Stage 1: Build the backend
FROM node:20-slim AS builder

WORKDIR /app

# Copy package files and install dependencies
COPY package*.json ./
RUN npm install --production

# Copy the rest of the backend code
COPY . .

# Stage 2: Create a slim image with Node.js
FROM node:20-slim

WORKDIR /app

# Copy built artifacts from the builder stage
COPY --from=builder /app /app

# Set environment variables for production
ENV NODE_ENV=production
ENV MONGODB_URI=mongodb://host.docker.internal:27017/?directConnection=true&serverSelectionTimeoutMS=2000&appName=mongosh+2.3.2  
ENV REDIS_HOST=redis

# Expose the backend port
EXPOSE 8000

# Start the application
CMD ["node", "server.js"]

