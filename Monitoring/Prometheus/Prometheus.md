# Prometheus

* <https://itnext.io/docker-swarm-monitoring-4dfe88c72d56>
* <https://github.com/opvizordz/docker-swarm-monitor>

## Exporter

* [BlackBox Exporter](https://github.com/prometheus/blackbox_exporter)

## How to?

* [Breaking down of one prometheus.yml file?](https://stackoverflow.com/questions/62390597/breaking-down-of-one-prometheus-yml-file)
  * prometheus.yml
  ```yaml
  - job_name: 'dummy' # it's mandatory
    file_sd_configs:
      - files:
        - /etc/prometheus/file_sd/*.json
  ```
  * json file
  ```json
  [
    {
      "targets": ["host:port"],
      "labels": {
        "job": "job_name",
        "environment": "test_env",
        "service": "test_service"
      }
    }
  ]
  ```
