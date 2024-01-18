# Docker-Compose Template for PHP Website
This project provides a Docker-Compose template to host a PHP website. It uses Docker to create two services: a web server and a database server.

## Project Structure
`apache2.Dockerfile`: Dockerfile for the Apache web server with PHP 8.1.
`database.Dockerfile`: Dockerfile for the MariaDB database server.
`docker-compose.yml`: Docker-Compose configuration file that defines the services.
`src/`: Directory containing the source code of the PHP website.
`src/.env`: Environment variables for the database.

## How to Run
  1. Install Docker and Docker-Compose on your machine if you haven't done so already.

  2. Clone this repository to your local machine.

  3. Navigate to the project directory.

  4. Run the following command to start the services:

  ```docker compose up -d```

This command will build the Docker images if they don't exist and start the services. The web server will be accessible at `http://localhost:85`

## Environment Variables
The `.env` file in the `src/` directory contains environment variables for the database. You can modify these variables as needed:

`DB_SERVER`: The database server name. Default is `mysql`.
`DB_ROOT_USER`: The root user for the database. Default is `root`.
`DB_ROOT_PASSWORD`: The root password for the database. Default is `qwerty`.
## License
This project is licensed under the MIT License. See the `LICENSE` file for more details.