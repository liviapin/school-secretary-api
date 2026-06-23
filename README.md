# School Secretary API

RESTful API built with .NET Core for managing a school secretary system. Handles students, classes, and enrollments with full CRUD operations.

## Tech Stack

- **.NET Core** with Entity Framework Core
- **PostgreSQL** (via Docker)
- **JWT** authentication
- **Swagger UI** for API documentation

## Getting Started

```bash
docker compose up
```

A default admin account is created automatically on first run:

| Field | Value |
|-------|-------|
| Email | `admin@admin.com` |
| Password | `Senha@123` |

### Authenticating in Swagger

1. Open Swagger UI at `http://localhost:8080/swagger`
2. `POST /api/auth/login` with the credentials above
3. Copy the JWT from the response
4. Click **Authorize** and enter: `Bearer <your_token>`

All protected routes are now available for testing.