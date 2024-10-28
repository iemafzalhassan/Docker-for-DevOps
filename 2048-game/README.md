# 2048-Game

### **Description**
2048-Game is a static web application that replicates the popular 2048 game. The game is built using HTML, CSS, and JavaScript. This project is containerized using Docker and runs a lightweight Python web server (Python 3.9 slim) to serve the game files. The application listens on port 8000.

### **Tech Stack**
- **Frontend**: HTML, CSS, JavaScript
- **Web Server**: Python’s built-in HTTP server
- **Containerization**: Docker (using Python slim image)

### **Features**
- A classic implementation of the 2048 game.
- Lightweight Python-based containerized web server.
- Simple to run and deploy using Docker.

### **Prerequisites**
- Docker (version 20.10 or higher)

### **Project Setup**

1. **Clone the repository**:
   ```bash
   git clone https://github.com/iemafzalhassan/2048-game.git
   cd 2048-game
   ```

2. **Build the Docker image**:
   ```bash
   docker build -t 2048-game .
   ```

3. **Run the Docker container**:
   ```bash
   docker run -d -p 8000:8000 --name 2048-game 2048-game
   ```

4. **Access the game**:
   Open your browser and go to `http://localhost:8000` to start playing the 2048 game.
