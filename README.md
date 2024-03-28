### Inception 42 Project
The aim of this project is to use dockerfile for the creation and management of custom images, microservices.

Writing dockerfile for the creation of containers.
How to write the docker-compose.yml file to make the containers work together in the correct order and make the system work the way we want.

##### How to run

run make or make up to start the docker-compose containers.
run make down to stop the containers.

##### About this project

For this project we need to setup a simple docker-compose network with the following containers:

NGINX with TLSv1.2 or TLSv1.3.
Wordpress + php-fpm (installed and configured).
MariaDB.

With the following volumes:

A volume that contains Wordpress database.
A volume that contains Wordpress website files.
Here is an example diagram of the expected result: </br>

<img width="580" alt="Ekran Resmi 2024-03-28 14 25 35" src="https://github.com/Ifmai/inception-docker/assets/94466351/cc13261e-9693-44ee-a95d-3074bb08266b">
