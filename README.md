# Docker is a beach! 🏖️🐋

Take advantage of useful Docker environments with preset configurations.

Most containers here will be part of a Docker Compose to facilitate deployment and integration with other services.

Below is a list of common commands shared by all instances. Refer to each folder for details and instructions on individual services.

## Cheatsheet 📜

- Run the Docker Compose service:

    ```shell
    docker compose up --build --force-recreate
    ```
The ```--build``` flag will force images to always have the latest contents, caching will still be done so if nothing changes the build is nearly instantaneous.

The ```--force-recreate``` flag will force containers to be restarted if they are already running.

Use the ```--detach``` flag to run the service in the background.

- Stop the Docker Compose service:

    ```shell
    docker compose down
    ```

- List all running containers from a Docker Compose:

    ```shell
    docker compose ps
    ```

- Get all logs from a Docker Compose:

    ```shell
    docker compose logs
    ```
