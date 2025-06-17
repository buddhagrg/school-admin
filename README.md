# Demo

[https://school-admin.xyz/](https://school-admin.xyz/)

**Admin**\
username: `admin@school-admin.xyz`\
password: `schooladmin`

# Docker

### Clone the repo

`https://github.com/buddhagrg/school-admin.git` \
`cd school-admin`

### Pull the docker images

`docker compose pull`

### Start the container

`docker compose up -d` \
`-d`: detached mode

### Stop the container

`docker compose stop`

### Remove containers

`docker compose down`

# Update Environment Variables in Docker Compose

To update `.env` file values for a specific service and ensure the changes take effect in its Docker container:

1.  **Edit the `.env` file:** Go to the service's folder (e.g., `/api`, `/frontend-vite`, `/frontend-next`) and update the `.env` file.

2.  **Restart the service:**
    ```bash
    docker compose stop <service_name>
    docker compose rm -s -f <service_name>
    docker compose up -d <service_name>
    ```
    **Example:**
    ```bash
    docker compose stop api
    docker compose rm -s -f api
    docker compose up -d api
    ```

# Want to check code?

Frontend(Landing Page): https://github.com/buddhagrg/school-admin-landing-page \
Frontend(Main App): https://github.com/buddhagrg/school-admin-frontend \
API: https://github.com/buddhagrg/school-admin-api \
DB: https://github.com/buddhagrg/school-admin-db

_**FYI:** You can add your own school, admin for that school and respective roles as per your need._
