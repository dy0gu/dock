# Postgres 🗄️

Basic PostgreSQL database.

- Perform a backup:

    ```shell
    docker exec <POSTGRES_CONTAINER_ID> pg_dump -c -U <POSTGRES_USER> <POSTGRES_DB> > backup.sql
    ```

- Restore a backup:

    ```shell
    cat backup.sql | docker exec -i <POSTGRES_CONTAINER_ID> psql -U <POSTGRES_USER> <POSTGRES_DB>
    ```

- Destroy all database data:

    ```shell
    docker compose down --volumes
    ```
