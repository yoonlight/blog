# OpenTelemetry

## Tempo

* <https://grafana.com/docs/tempo/latest/getting-started/>

## Jaeger

* <https://www.jaegertracing.io/docs/1.29/getting-started/#all-in-one>
* Dokcer-Compose
  ```yaml
    jaeger:
      image: jaegertracing/all-in-one:1.29
      environment:
        - COLLECTOR_ZIPKIN_HOST_PORT=:9411
      ports:
        - 5775:5775/udp
        - 6831:6831/udp
        - 6832:6832/udp
        - 5778:5778
        - 16686:16686 # Web Dashboard
        - 14250:14250
        - 14268:14268
        - 14269:14269
        - 9411:9411
  ```

## Reference

* <https://opentelemetry.io/docs/instrumentation/js/>

## Example

### Javascript

* <https://github.com/mnadeem/nodejs-opentelemetry-tempo>
* <https://github.com/open-telemetry/opentelemetry-js-contrib/tree/main/examples>
* <https://github.com/open-telemetry/opentelemetry-js/tree/main/examples>

