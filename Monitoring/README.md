# Monitoring

## Elastic
* ElasticSearch
* Elastic APM
  * <https://notificare.com/blog/2021/01/22/Monitoring-Performance-With-Elastic/>
  * <https://saramin.github.io/2020-03-24-elastic-apm-2/>
  * <https://saramin.github.io/2020-03-24-elastic-apm-1/>
  * <https://itnext.io/distributed-tracing-in-your-kibana-with-nodejs-610c9f07b4b4>
* Kibana
* Logstash
* File Beats

## Prometheus
* [Prometheus](<Prometheus/Prometheus.md>)
* [Grafana](<Prometheus/Grafana.md>)
* Loki
  * [Installation](https://grafana.com/docs/loki/latest/installation/docker/)
  * [Configure the logging driver for a Swarm service or Compose](https://grafana.com/docs/loki/latest/clients/docker-driver/configuration/#configure-the-logging-driver-for-a-swarm-service-or-compose)
  * ```YAML
    version: "3"
      services:
        grafana:
          image: grafana/grafana
          logging:
            driver: loki
            options:
              loki-url: http://host.docker.internal:3100/loki/api/v1/push
      ```
  * [Docker Driver](https://grafana.com/docs/loki/latest/clients/docker-driver/)
    ```shell
    docker plugin install grafana/loki-docker-driver:latest --alias loki --grant-all-permissions
    ```
    Apply Success Check
    ```shell
    docker plugin ls
    ```
* Alertmanager
    * [Alert Rules](https://awesome-prometheus-alerts.grep.to/rules)
