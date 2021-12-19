# Docker


## DockerFile Default Setting

```Dockerfile
FROM ubuntu:18.04
# timezone setting
ARG DEBIAN_FRONTEND=noninteractive
ENV TZ=Asia/Seoul

# Change Location of APT Archive
RUN cd /etc/apt && \
  sed -i 's/archive.ubuntu.com/mirror.kakao.com/g' sources.list

RUN apt update -y

RUN apt install -y sudo vim wget tzdata
RUN apt install -y apache2

CMD [ "bash" ]
```
### How to use?
* [Is it safe to clean docker/overlay2/](https://stackoverflow.com/questions/46672001/is-it-safe-to-clean-docker-overlay2)

### Ref.
* <https://www.leafcats.com/242>
* <https://stynxh.github.io/2020-07-26-set-timezone-when-ubuntu-docker-image-build/>
* [Use a pre-existing network](https://docs.docker.com/compose/networking/#use-a-pre-existing-network)
  ```yaml
  services:
    # ...
  networks:
    default:
      external: true
      name: my-pre-existing-network  
  ```

* [](https://github.com/ofstudio/docker-compose-scale-example)
* [](https://medium.com/@vinodkrane/microservices-scaling-and-load-balancing-using-docker-compose-78bf8dc04da9)
* [](https://codeburst.io/scaling-out-with-docker-and-nginx-8eda9fb1654c)
* [](https://stackoverflow.com/questions/50203408/docker-compose-scale-x-nginx-conf-configuration)
* 
