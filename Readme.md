oxid-docker-compose
===================

The next generation container composium to run oxid esales

If you are looking for a well maintained, suported and stable development environment please try out the official
oxvm https://github.com/OXID-eSales/oxvm_eshop

Oxvm is great peace of software, and getting better every day. But the goal of this project is to build a even better development environment: 
- based on seperated components.
- faster when running oxid
- faster when reconfiguring things
- more independet components (vagrant,nginx,mysql,elasticsearch,memcached,redis...,php)

Current state
=============

The docker compose file is a prove of concept.
It is able to show the setup page of oxid, but not yet ready to install oxid.

Getting started
===============
Join the team:
* [![Join the chat at https://gitter.im/keywan-ghadami/oxid-docker-compose](https://badges.gitter.im/keywan-ghadami/oxid-docker-compose.svg)](https://gitter.im/keywan-ghadami/oxid-docker-compose?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
* Or create bugtickets with any question


* git clone --recursive git@github.com:keywan-ghadami/oxid-docker-compose.git
* in the copy config.inc.php.dist => config.inc.php 
* Install Docker https://docs.docker.com/engine/installation/
* Install Docker Compose https://docs.docker.com/compose/install/
* run docker compose start
* get the name of the php container by running: docker compose ps
* asume the name is oxid-docker-compose_php_1 the run
  * docker exec -i -t oxidvargant_php_1 bash
  * run composer install -o --no-dev
* open your browser http://localhost

