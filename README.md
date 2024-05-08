# Webshop Experiment With Payload

## Accessing the Payload admin panel:

1. Start docker
1. `docker compose up -d`
1. `yarn dev`
1. Open your web browser and visit `http://localhost:3000/`.

## Accessing the database

### Using psql

Interact directly with the PostgreSQL database using the psql cli:

1. Access the shell of the running PostgreSQL container:
  ```bash
  docker exec -it postgres bash
  ```
2. Once inside the container, connect to the database:
```bash
psql -U user123 -d webshop
```

### Using Adminer

1. Open your web browser and visit `http://localhost:8080/`.
2. Log in with the following credentials:
    - System: `PostgreSQL`
    - Server: `postgres` 
    - Username: `user123`
    - Password: `password123`
    - Database: `webshop`
