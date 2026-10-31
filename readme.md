# PSUSphere – Docker Containerization

## Description

This project demonstrates the containerization of the PSUSphere Django application using Docker and Docker Compose.

## Requirements

- Docker Desktop
- Docker Compose

## Project Structure

- `Dockerfile` – Instructions for building the Docker image.
- `docker-compose.yml` – Configuration for building and running the application locally.
- `requirements.txt` – Python dependencies.
- `.dockerignore` – Files excluded from the Docker build.
- `for_client/docker-compose.yml` – Configuration for pulling and running the Docker Hub image.

## Run Locally

Navigate to the project directory containing the Dockerfile and manage.py.

Build the Docker image:

```bash
docker compose build
```
Start the application:

```bash
docker compose up
```

Open the application:

http://localhost:8000

## View Logs

```bash
docker compose logs -f web
```

## Check Containers

```bash
docker compose ps
```

## Stop the Application

```bash
docker compose down
```

## Docker Hub

Docker image:

`micahana/psusphere:latest`

## Run Using Docker Hub

Navigate to the `for_client` directory:

```bash
cd for_client
```

Pull the image:

```bash
docker compose pull
```

Start the application:

```bash
docker compose up -d
```

Open:

http://localhost:8000


## Authors

[Milcahana Q. Montemayor](https://github.com/micahana4)  
[Gabriel Jansmhir M. Ibarra](https://github.com/cojjeeee)

