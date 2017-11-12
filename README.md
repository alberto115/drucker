# Docker NGINX compose

## Introduction

Docker compose kick-starting set.

## Set up

* **NGINX**: Latest from docker hub.
* **PHP 7-fpm**: Optimized version 7.1.10
* **Percona**: Version 5.7

## Running the project

Get the project with composer:
`composer create-project abesiyo/drucker`

Uncomment the last 3 lines of the settings.php to include the local.settings.php with the docker configuration.

Before running docker, you can do some changes on .env to fit the configuration to your project.

Run docker compose
`docker-compose up -d`

If you have the domain in your hosts file, you should be able to hit the site on **https://vm.localhost/**

## Other useful commands
Stop docker stack
`docker-compose stop`

Destroy the whole docker stack. This also delete the database.
`docker-compose down`
