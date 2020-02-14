![image](images/rfc.png)

* [Intro](#intro)
* [Build MQ Dockerfile](#mq-dockerfile)
* [Build Connector Instance Dockerfile](#connector-dockerfile)
* [Docker Compose Setup](#docker-compose)
* [Prerequisities](#prerequisites)

 intro
 Initially a clone of the confluent examples [cp-all-in-one](https://github.com/confluentinc/examples/tree/5.3.1-post/cp-all-in-one)
 

 mq-dockerfile
 I will have to configure multiple connector instances into the cluster, as docker images (one image for each connector instance)
 Using the MQ container image from [here](https://github.com/ibm-messaging/mq-container)
 
 connector-dockerfile
 docker-compose
 
 
 Prerequisites

* Env var `CONFLUENT_HOME=/path/to/confluentplatform`
* Env var `PATH` includes `$CONFLUENT_HOME/bin`

For Docker: demos have been validated with
* [Docker](https://docs.docker.com/install/) version 17.06.1-ce
* [Docker Compose](https://docs.docker.com/compose/install/) version 1.14.0 with Docker Compose file format 2.1
