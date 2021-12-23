# Loki

* [Installation](https://grafana.com/docs/loki/latest/installation/docker/)
* Docker Compose Script
  ```YAML
  services:
    loki:
      image: grafana/loki:2.4.0
      ports:
        - "3100:3100"
      command: -config.file=/etc/loki/local-config.yaml  
  ```
* [Configure the logging driver for a Swarm service or Compose](https://grafana.com/docs/loki/latest/clients/docker-driver/configuration/#configure-the-logging-driver-for-a-swarm-service-or-compose)
  ```YAML
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
  * Add to Docker
  ```shell
  docker plugin install grafana/loki-docker-driver:latest --alias loki --grant-all-permissions
  ```
  * Apply Success Check
  ```shell
  docker plugin ls
  ```
* [running loki and grafana on docker swarm](https://drailing.net/2020/06/running-loki-and-grafana-on-docker-swarm/)
  * log collector: docker-driver vs promtail
