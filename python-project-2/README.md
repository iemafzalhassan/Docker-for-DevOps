# Python-Project-2

### Description
Python-Project-2 is a basic web application built using the Flask framework. The application serves an `index.html` file as the homepage and runs on port 9001. The project is containerized using Docker and uses a lightweight Python image (`python:3.10-alpine`) for efficient deployment.

### Project Structure
- `app.py`: The main Flask application file, responsible for handling routes and rendering templates.
- `templates/`: Contains the HTML templates for the web app.
  - `index.html`: The homepage of the web application.
- `requirements.txt`: Lists the dependencies for the Python project.

### Tech Stack
- **Backend**: Flask (Python)
- **Web Server**: Flask's development server
- **Containerization**: Docker (using Python Alpine image)

### Features
- Basic Flask application serving an HTML page.
- Lightweight containerized Python app for fast startup and low memory usage.

### Prerequisites
- [Docker](https://www.docker.com/) (version 20.10 or higher)
- [Python](https://www.python.org/downloads/) (if running the app outside Docker)
- `pip` for installing Python dependencies

### Project Setup

1. **Clone the repository:**
   ```bash
   git clone https://github.com/iemafzalhassan/Docker-for-DevOps.git
   cd Docker-for-DevOps/Python-Project-2
