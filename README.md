# docker-etherpad

## Quickstart

Start your own instance of Etherpad by running

    docker-compose run
    
Prerequisite: Working docker host [Installing docker](https://docs.docker.com/engine/installation/)

To prepare your environment you should also copy the file `.env-example` to a file called `.env`:

    cp .env-example .env
  
In the `.env` file, adjust the user and password for the etherpad admin user:

    ETHERPAD_ADMIN_USER=youradminuser
    ETHERPAD_ADMIN_PASSWORD=youradminpassword

Once the docker container was started with `docker-compose run -d`, you should be able to work with etherpad at http://localhost:9001/
The etherpad admin area can be opened at http://localhost:9001/admin/

## About

This docker-compose file uses the docker image provided by indiehosters:
https://github.com/indiehosters/docker-etherpad

The image pulls the latest etherpad version from GitHub at https://github.com/ether/etherpad-lite
