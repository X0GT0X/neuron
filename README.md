# Neuron - playground project with microservices and DDD 

## ToC
- [Requirements](#requirements)
- [How to run locally](#how-to-run-locally)
- [Available hosts (dev)](#available-hosts-dev)
- [How to connect to local database](/docs/DATABASE.md)

## Requirements
1. Install [Docker](https://docker.com/) and [docker-compose](https://docs.docker.com/compose/install/)
2. Install [mkcert](https://github.com/FiloSottile/mkcert) for creating trusted ssh certificates locally.
3. Run `git submodule update --init --recursive` to fetch all microservices.

## How to run locally
1. Run `mkcert -install` if you didn't have mkcert tool before.
2. Run `make ssl-certs` to generate ssl certificates for application.
3. Run `make init` to build all microservices containers. 
4. Run `make start` to start all microservices.

## Available hosts (dev)
- [RabbitMQ Dashboard - https://rabbit.neuron.localhost/](https://rabbit.neuron.localhost/)
- [Proxy Dashboard - https://proxy.neuron.localhost/](https://proxy.neuron.localhost/)