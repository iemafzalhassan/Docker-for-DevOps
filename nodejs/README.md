# Docker for DevOps

Welcome to the **Docker for DevOps** repository! This project is designed to provide hands-on practice for aspiring DevOps engineers by leveraging Docker to containerize a simple Node.js application.

## Overview

This project includes a basic Express.js application that serves a friendly greeting to users. By using Docker, you can easily run and manage this application in a containerized environment, helping you to understand the fundamentals of containerization and DevOps practices.

## Getting Started

### Prerequisites

Before you begin, ensure you have the following installed on your machine:

- [Docker](https://www.docker.com/get-started)
- [Node.js](https://nodejs.org/en/download/) (for development purposes)

### Clone the Repository

Start by cloning this repository to your local machine:

```bash
git clone https://github.com/iemafzalhassan/Docker_for_DevOps.git
```

```bash
cd Docker_for_DevOps
```

### Build the Docker Image

To build the Docker image for the application, run:

```bash
docker build -t nodejs-app .
```

### Run the Docker Container

Once the image is built, you can run the container using the following command:

```bash
docker run -p 5001:5001 nodejs-app
```

### Access the Application

Open your web browser and navigate to `http://localhost:5001` to see the greeting message:

```html
<h2>Hello Aspiring DevOps Engineers!</h2>
```

## Project Structure

The project consists of the following files:

- `index.js`: The main application file that sets up the Express server.
- `package.json`: Contains metadata about the application and its dependencies.
- `Dockerfile`: Defines the instructions for building the Docker image.

## Dependencies

This project uses the following dependencies:

- **Express**: A minimal and flexible Node.js web application framework.

```json
{
  "dependencies": {
    "express": "^4.21.1"
  }
}
```

## License

This project is licensed under the [MIT License](LICENSE).

