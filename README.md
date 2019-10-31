# Envoy Proxy Demos

Set of demos to demostrate Envoy features running together with K8s API and Prometheus.

## Getting started

Choose between `Prometheus` or `K8s API` and run the below command:

```sh
./deploy.sh <folder-name>
```

## Circuit Breaker

[Circuit Breaking](https://www.envoyproxy.io/learn/circuit-breaking) lets you configure failure thresholds that ensure safe maximums after which these requests stop. This allows for a more graceful failure, and time to respond to potential issues before they become larger.

## Fault Injection

Fault injection is a technique for improving the coverage of a test by introducing faults to test code paths, in particular error handling code paths, that might otherwise rarely be followed. The filter ( `http_filters` in the demo ) can be used to inject delays (`delay` folder) and abort requests (`abort` folder) with user-specified error codes.

## Timeouts and Retry

TBD