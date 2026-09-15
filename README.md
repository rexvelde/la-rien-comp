# la-rien-comp
Tool to host typewriting competitions defined by our own rules.

## Docker

Run the full local stack:

```sh
docker compose up --build
```

Services:

- Frontend: http://localhost:5173
- Backend: http://localhost:8080
- Swagger UI: http://localhost:8080/swagger-ui/index.html
- MySQL: `localhost:3306`

Project layout:

```text
backend/              Spring Boot API
frontend/             Vue + TypeScript app
docker-compose.yml    Local orchestration
docker/mysql/init/    MySQL init scripts
```

MySQL runtime files are stored in the `mysql-data` Docker volume, not in the repo.
