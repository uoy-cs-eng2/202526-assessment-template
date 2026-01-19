# ENG2 2025-26 starting template

Starting code for an assessment on creating reactive computation components to implement a home automation scenario.

## Configuration for Docker Engine 29

Until [this issue](https://github.com/micronaut-projects/micronaut-test-resources/issues/941) is fixed, you will need to manually tell Testcontainers which Docker API version to use:

```shell
echo api.version=1.44 > $HOME/.docker-java.properties
```
