# What do we have here?
Using this setup you can setup wordpress running with MariaDB, PHP7 on your own computer or on server, software will run from port 8080 and database port 8081 you can change these in `docker-compose.yml` file if you like. Additionaly there's uploads.yml where you can setup e.g. `upload_max_filesize`.
Docker will create wordpress folder volume(if not already there), so changes you make there will be effected wordpress running in container.

# Prerequisite
You will need [docker](https://docs.docker.com/install/) and [docker compose](https://docs.docker.com/compose/install/) installed on your system.
Create docker hub account and in commandline login to hub `docker login` with your credentials.

# Start up your WordPress
Clone repo and do your changes in docker-compose.yml file, e.g. change port numbers or in uploads.ini file change upload_max_filesize.
Then you can just hit `docker-compose up -d` and docker dose rest.
After docker is done you can finalize your WordPress install from `localhost:8080` or what ever port you change in place on 8080 same goes with MariaDB 8081 port.
