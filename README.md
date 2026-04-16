# Demo

Simple Spring Boot application with local development backed by MariaDB in Docker Compose.

## Prerequisites

- Java 17
- Docker and Docker Compose

## Local Development

Start the database:

```bash
docker compose up -d
```

Run the Spring Boot app locally:

```bash
mvn spring-boot:run
```

The application uses the database configured in [`src/main/resources/application.yml`](src/main/resources/application.yml):

- Host: `localhost`
- Port: `3306`
- Database: `demo`
- Username: `demo`
- Password: `demo`

## Useful Commands

Run tests:

```bash
mvn test
```

Stop the database:

```bash
docker compose down
```
