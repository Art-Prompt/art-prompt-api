# Art Prompt API

A simple API that generate an art prompt that remain the same for 24 hours. Goal is to help practice artistic creativity by drawing
from a prompt daily.

## Dev Setup

### Pull Ollama and Redis images

```bash
    docker pull ollama/ollama
    docker pull redis
```

### Add .env file with the following variables:

- MONGODB_URI={get from mongo db}
- OLLAMA_URL={host:port_number}

Note: Current IP need to be add in MonogoDB dashboard to
art prompt clustor for access.

### Run Docker Compose Build

```bash
    docker-compose up --build
```

Note: If there is a connection issue with Ollama or Redis service
with Docker Compose, use host.docker.internal instead of localhost

### If the containers been build, use the following commands to run the API

```bash
    docker-compose up backend
```

```bash
    docker-compose up ollama
```
