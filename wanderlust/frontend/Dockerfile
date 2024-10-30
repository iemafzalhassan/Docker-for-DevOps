# Stage 1: Build the frontend
FROM node:20 AS builder

WORKDIR /app

# Copy package files and install dependencies
COPY package*.json ./
RUN npm install

# Copy the rest of the frontend code
COPY . .

# Build the frontend
RUN npm run build

# Stage 2: Serve the built files
FROM nginx:alpine

# Copy the built files from the builder stage to the NGINX HTML directory
COPY --from=builder /app/dist /usr/share/nginx/html

# Expose the frontend port
EXPOSE 80

# Start NGINX
CMD ["nginx", "-g", "daemon off;"]

