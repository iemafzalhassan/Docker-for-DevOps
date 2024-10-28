# Use a lightweight Python base image
FROM python:3.9-slim

# Set the working directory to /app
WORKDIR /app

# Copy the current directory contents into the container at /app
COPY . /app

# Expose port 8000 for HTTP traffic
EXPOSE 8000

# Run Python's built-in HTTP server to serve the content
CMD ["python3", "-m", "http.server", "8000"]
