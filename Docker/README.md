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
