<p align="center">
    <a href="https://github.com/quarkus-qe/quarkus-test-framework/pulse" alt="Activity">
        <img src="https://img.shields.io/github/commit-activity/m/quarkus-qe/quarkus-test-framework"/></a>
    <a href="https://github.com/quarkus-qe/quarkus-test-framework/actions/workflows/daily.yaml" alt="Build Status">
        <img src="https://github.com/quarkus-qe/quarkus-test-framework/actions/workflows/daily.yaml/badge.svg"></a>
    <a href="https://github.com/quarkus-qe/quarkus-test-framework" alt="Top Language">
        <img src="https://img.shields.io/github/languages/top/quarkus-qe/quarkus-test-framework"></a>
</p>

Welcome to the Quarkus Test Framework wiki!

The framework is designed using Extension Model architecture patterns, so supporting additional features or deployment options like Kubernetes or AWS is just a matter of implementing extension points and adding dependencies into the classpath.

Main features:
- Easily deploy multiple Quarkus applications and third party components in a single scenario
- Write the test scenario once and run it everywhere (cloud, bare metal, etc)
- Developer and Test friendly
- Quarkus features focused (allow to define custom source classes, build/runtime properties, etc)
- Test isolation: for example, in OpenShift or Kubernetes, tests will be executed in an ephemeral namespace 

Content:
- [Getting Started](https://github.com/quarkus-qe/quarkus-test-framework/wiki/1.-Getting-Started)
- [Configuration](https://github.com/quarkus-qe/quarkus-test-framework/wiki/2.-Configuration)
- [Architecture](https://github.com/quarkus-qe/quarkus-test-framework/wiki/3.-Architecture)
- [Services](https://github.com/quarkus-qe/quarkus-test-framework/wiki/4.-Services)
- [Containers](https://github.com/quarkus-qe/quarkus-test-framework/wiki/5.-Containers)
- [OpenShift](https://github.com/quarkus-qe/quarkus-test-framework/wiki/6.-Openshift)
- [Kubernetes](https://github.com/quarkus-qe/quarkus-test-framework/wiki/7.-Kubernetes)
- [Advanced Quarkus modes](https://github.com/quarkus-qe/quarkus-test-framework/wiki/8.-Advanced-Quarkus-Modes)
- [Scenario Tracing/Metrics](https://github.com/quarkus-qe/quarkus-test-framework/wiki/9.-Scenario-Tracing-And-Metrics)

Summary of features and compability:

| Features | [Baremetal](https://github.com/quarkus-qe/quarkus-test-framework/wiki/1.-Getting-Started) | [Native](https://github.com/quarkus-qe/quarkus-test-framework/wiki/1.-Getting-Started#native) | [OpenShift](https://github.com/quarkus-qe/quarkus-test-framework/wiki/6.-Openshift#usage) | [Kubernetes](https://github.com/quarkus-qe/quarkus-test-framework/wiki/7.-Kubernetes#usage) |
|----------|:------:|:------:|:------:|:------:|
| [@QuarkusApplication](https://github.com/quarkus-qe/quarkus-test-framework/wiki/1.-Getting-Started#buildruntime-properties) | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |
| [@DevModeQuarkusApplication](https://github.com/quarkus-qe/quarkus-test-framework/wiki/8.-Advanced-Quarkus-Modes#quarkus-dev-mode) | :heavy_check_mark: | :x: | :x: | :x: |
| [@RemoteDevModeQuarkusApplication](https://github.com/quarkus-qe/quarkus-test-framework/wiki/8.-Advanced-Quarkus-Modes#quarkus-remote-dev-mode) | :heavy_check_mark: | :x: | :heavy_check_mark: | :heavy_check_mark: |
| [@GitRepositoryQuarkusApplication](https://github.com/quarkus-qe/quarkus-test-framework/wiki/1.-Getting-Started#remote-repositories) | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |
| [@Container](https://github.com/quarkus-qe/quarkus-test-framework/wiki/5.-Containers) | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |
| [@KafkaContainer(vendor = STRIMZI)](https://github.com/quarkus-qe/quarkus-test-framework/wiki/5.-Containers#strimzi) | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :x: |
| [@KafkaContainer(vendor = CONFLUENT)](https://github.com/quarkus-qe/quarkus-test-framework/wiki/5.-Containers#confluent) | :heavy_check_mark: | :heavy_check_mark: | :x: | :x: |
| [@AmqContainer](https://github.com/quarkus-qe/quarkus-test-framework/wiki/5.-Containers#amq-containers) | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :x: |
| [@JaegerContainer](https://github.com/quarkus-qe/quarkus-test-framework/wiki/5.-Containers#jaeger-containers) | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :x: |
| [@Operator](https://github.com/quarkus-qe/quarkus-test-framework/wiki/6.-Openshift#operators) | :x: | :x: | :heavy_check_mark: | :x: |
