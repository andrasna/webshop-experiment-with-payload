# Webshop Experiment with Payload

## Accessing the Database

### Using psql

Interact directly with the PostgreSQL database using the psql cli:

1. Access the shell of the running PostgreSQL container:
  ```bash
  docker exec -it postgres bash
  ```
2. Once inside the container, connect to the webshop_experiment database:
```bash
psql -U user -d webshop_experiment
```

### Using Adminer

1. Open your web browser and visit `http://localhost:8080/`.
2. Log in with the following credentials:
    - System: `PostgreSQL`
    - Server: `postgres` 
    - Username: `user`
    - Password: `password`
    - Database: `webshop_experiment`
