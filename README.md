# ENG2 2025-26 starting template

Starting code for an assessment on creating reactive computation components to implement a home automation scenario.

## Configuration for Docker Engine 29+

If Docker Desktop is running normally and you see this error message while trying to run tests or start the application:

```
Caused by: java.lang.IllegalStateException: Could not find a valid Docker environment. Please see logs and check configuration
```

Then you may be affected by [this issue](https://github.com/micronaut-projects/micronaut-test-resources/issues/941).
Until it is fixed, you will need to manually tell Testcontainers which Docker API version to use.
On a Linux/Mac environment, you will need to use:

```shell
echo api.version=1.44 > $HOME/.docker-java.properties
```

## CI for Part 1

The repository includes a [Github CI YAML](./.github/workflows/gradle.yml) workflow file with the basic commands needed to perform continuous integration on the Part 1 work.

Some of the entries are commented out, as they will only work once you have done sufficient work on the microservices and/or the end-to-end tests.
We suggest you uncomment them when appropriate.
