# Monitoring

## Elastic
* ElasticSearch
* Elastic APM
* Kibana
* Logstash
* File Beats

## Prometheus
* Prometheus
* Grafana
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
