# cf-SpringBootTrader-extras
Extra tools to work with the [cf-SpringBootTrader](https://github.com/dpinto-pivotal/cf-SpringBootTrader) project.

This project provides a few extra tools for [cf-SpringBootTrader](https://github.com/dpinto-pivotal/cf-SpringBootTrader), such as:

1. Discovery Server:

This is a discovery server for microservices to register and find out about other services. Some platforms provide one of these, such as Pivotal Cloud Foundry, others don't. Also, if you want to test the [cf-SpringBootTrader](https://github.com/dpinto-pivotal/cf-SpringBootTrader) locally, you'll need to run one of these.

2. Config Server:

This is a config server for microservices.

3. Turbine server

This is a turbine and hystrix dashboard server to display circuit breaker information. It uses the discovery server above to find out where and which services to grab information from.
