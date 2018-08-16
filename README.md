[![Build Status][circleci-image]][circleci-url]

# Microservices

This demo application shows how a microservices architecture can be implemented and applied!
This demo application covers the following topics:

  * front-end client
  * back-end services
  * REST, gRPC, and GraphQL
  * logging, metrics, and tracing
  * api gateway and web gateway
  * containerization and orchestration

## Services

  * [react-client](./services/react-client)
  * [site-service](./services/site-service)
  * [sensor-service](./services/sensor-service)
  * [switch-service](./services/switch-service)
  * [graphql-server](./services/graphql-server)

## Up & Running

  * [docker-compose](./compose)
  * [docker swarm](./swarm)
  * [kubernetes](./kubernetes)

## Architecture

![system architecture](./docs/architecture.png)


[circleci-url]: https://circleci.com/gh/moorara/microservices-demo/tree/master
[circleci-image]: https://circleci.com/gh/moorara/microservices-demo/tree/master.svg?style=shield
