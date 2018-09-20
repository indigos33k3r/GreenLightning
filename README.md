NOTE: After clone of this project the following 2 git commands must be run in order to also clone the source
* git submodule init
* git submodule update

# Green Lightning
Green Lightning is an embeddable high-performance microservice framework with built-in HTTP and MQTT support.

## How is it different?
Green Lightning is built from the ground-up to be garbage-free, lock-free, and security-first. It is capable of running directly on Compact-1 Java Virtual Machines with no additional configuration.

The framework uses a declarative event-driven actor model, making code simpler and easier to maintain. Because of this declarative model, operational logic like thread synchronization, exception handling, and null object conditions are handled by the framework and completely removed from your business logic. This lets users write logic that is multithreaded *and* asynchronous without ever scheduling a single task or creating a single lock.

Green Lightning supports fine-grained telemetry information published via a built-in web server which can be enabled or disabled with a single flag. When enabled, this server allows users to inspect live metrics about class-level CPU utilization and end-to-end data throughput - all without any specialized build or deployment.

## Performance
Benchmarks for Green Lightning are provided by the [GreenLoader project. Below is a graph that compares the latency by percentile of Green Lightning and several other web services frameworks with request logging and telemetry enabled.

![Green Lightning Benchmark](https://objectcomputing.github.io/GreenLightning/assets/images/benchmark.png)
