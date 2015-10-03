# cf-SpringBootTrader-extras
Extra tools to work with the [cf-SpringBootTrader](https://github.com/dpinto-pivotal/cf-SpringBootTrader) project.

This project provides a few extra tools for [cf-SpringBootTrader](https://github.com/dpinto-pivotal/cf-SpringBootTrader), such as:

1. Discovery Server:

This is a discovery server for microservices to register and find out about other services. Some platforms provide one of these, such as Pivotal Cloud Foundry, others don't. Also, if you want to test the [cf-SpringBootTrader](https://github.com/dpinto-pivotal/cf-SpringBootTrader) locally, you'll need to run one of these.

2. Config Server:

This is a config server for microservices to manage the configuration for all the services backed by a git repository.

3. Turbine server

This is a turbine and hystrix dashboard server to display circuit breaker information. It uses the discovery server above to find out where and which services to grab information from.

##How to run

###1. Discovery Server:
####To run locally
Run the project using `gradlew bootRun` or build the project with `gradlew build` and then run with `java -jar build/libs/registry-0.0.1.jar`

####To run in Pivotal Cloud Foundry
Build the project using `gradlew build` and then *push* the `build/libs/registry-0.0.1.jar` to the cloud.

You may want to create a manifest file to set things such as memory and routes.
