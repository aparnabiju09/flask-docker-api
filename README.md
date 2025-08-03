# flask-docker-api
# Flask Docker To-Do API

A simple REST API built with Flask to manage a to-do list, containerized using Docker.

## Features

- **GET /tasks**: Retrieve the list of tasks
- **POST /tasks**: Add a new task

## Getting Started

### Prerequisites

- [Docker](https://www.docker.com/get-started) installed

### Run with Docker

1. Build the Docker image:

```bash
docker build -t flask-docker-api .

docker run -p 5000:5000 flask-docker-api

### GET /tasks
curl http://localhost:5000/tasks

### POST /tasks
curl -X POST -H "Content-Type: application/json" -d '{"task": "Study Docker"}' http://localhost:5000/tasks

### Project Structure
flask-docker-api/
├── app.py
├── requirements.txt
└── Dockerfile




