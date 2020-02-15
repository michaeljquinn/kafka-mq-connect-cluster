![image](images/rfc.png)

* [Intro](#intro)
* [Build MQ Dockerfile](#mq-dockerfile)
* [Build Connector Instance Dockerfile](#connector-dockerfile)
* [MQ Message injector](#injector)
* [Docker Compose Setup](#docker-compose)
* [Prerequisities](#prerequisites)
* [References](#references)

 intro
 Initially a clone of the confluent examples [cp-all-in-one](https://github.com/confluentinc/examples/tree/5.3.1-post/cp-all-in-one)
 
plan
1 - cp all in one dockerfile, without connector instance


 mq-dockerfile
 I will have to configure multiple connector instances into the cluster, as docker images (one image for each connector instance)
 Using the MQ container image from [here](https://github.com/ibm-messaging/mq-container)
 
 mq connect cluster
 A cluster of mq source connectors (sourcing messages from MQ into kafka)
 Each connector instance is a single worker
 
#### connector-dockerfile
 
#### injector
 
#### docker-compose



 
 
#### Prerequisites

* Env var `CONFLUENT_HOME=/path/to/confluentplatform`
* Env var `PATH` includes `$CONFLUENT_HOME/bin`

For Docker: demos have been validated with
* [Docker](https://docs.docker.com/install/) version 17.06.1-ce
* [Docker Compose](https://docs.docker.com/compose/install/) version 1.14.0 with Docker Compose file format 2.1

#### References
* [Medium article](https://medium.com/clay-one/kafka-connect-cluster-an-introduction-26522e72a9af)
* [Confluent-Kafka Connect Architecture](https://docs.confluent.io/current/connect/design.html)
* [Confluent connect on docker](https://docs.confluent.io/5.0.0/installation/docker/docs/installation/connect-avro-jdbc.html)
* [comoposerize your docker run commands](https://composerize.com/)
