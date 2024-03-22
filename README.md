# open6gc with docker-compose

The open6gc project offers all its services in Docker. In this repository, you will find a docker compose version of open6gc version stage beta.

# Getting Started

Follow this documentation to run open6gc components within Docker.

## Requirements

- Docker Engine (if you are using Docker Desktop, it requires version 4.22+)
- Docker Compose 2.20.3+

## open6gc compose main file

The `docker-compose.yaml` contains all setup, by importing the separated files.

```yaml
include: 
  - network.yaml
  - mongo.yaml
  - rabbitmq.yaml
  - monitoring.yaml
```

## Run open6gc

Clone this repository, open compose folder and run the application:

```bash
cd compose/
```

```bash
docker compose up -d
```
