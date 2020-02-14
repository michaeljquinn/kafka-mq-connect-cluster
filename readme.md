![image](images/rfc.png)

* [Intro](#intro)
* [Build MQ Dockerfile](#mq-dockerfile)
* [Build Connector Instance Dockerfile](#connector-dockerfile)
* [Docker Conpose Setup](#docker-compose)
* [Prerequisities](#prerequisites)

 intro

 mq-dockerfile
 connector-dockerfile
 docker-compose
 Prerequisites

For local installs:

* Download [Confluent Platform 5.4](https://www.confluent.io/download/?utm_source=github&utm_medium=demo&utm_campaign=ch.examples_type.community_content.top)
* Env var `CONFLUENT_HOME=/path/to/confluentplatform`
* Env var `PATH` includes `$CONFLUENT_HOME/bin`
* Each demo has its own set of prerequisites as well, documented individually in each demo

For Docker: demos have been validated with

* [Docker](https://docs.docker.com/install/) version 17.06.1-ce
* [Docker Compose](https://docs.docker.com/compose/install/) version 1.14.0 with Docker Compose file format 2.1
