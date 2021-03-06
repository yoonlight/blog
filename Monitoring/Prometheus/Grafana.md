# Grafana

## Install

* Docker-Compose
  ```yaml
  grafana:
    image: grafana/grafana
    ports:
      - "3000:3000"
    volumes:
      - grafana_data:/var/lib/grafana
    #  - /root/monitoring/grafana/datasource.yaml:/etc/grafana/provisioning/datasources/datasource.yaml
  ```



## Dashboards

* cAdvisor
  * <https://grafana.com/grafana/dashboards/14282>
* Loki
  * <https://grafana.com/grafana/dashboards/12019>
* Node.js
  * <https://grafana.com/grafana/dashboards/11159>
* Node Exporter
  * <https://grafana.com/grafana/dashboards/1860>
  * <https://grafana.com/grafana/dashboards/13978>
* Black Box Exporter
  * <https://grafana.com/grafana/dashboards/7587>

## Datasources

* Prometheus
  * <https://grafana.com/docs/grafana/latest/datasources/prometheus/>
* MySQL
  * <https://grafana.com/docs/grafana/latest/datasources/mysql/#configure-the-data-source-with-provisioning>
* Loki
  * <https://grafana.com/docs/grafana/latest/datasources/loki/#configure-the-data-source-with-provisioning>
* Alertmanager
  * <https://grafana.com/docs/grafana/latest/datasources/alertmanager/>
* Jaeger
  * <https://grafana.com/docs/grafana/latest/datasources/jaeger/>
  ```yaml
  datasources:
    - name: Jaeger
    type: jaeger
    uid: jaeger-spectra
    access: proxy
    url: http://jaeger:16686/
  ```
