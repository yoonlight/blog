# Docker


## DockerFile Default Setting

```Dockerfile
FROM ubuntu:18.04
ARG DEBIAN_FRONTEND=noninteractive
ENV TZ=Asia/Seoul
RUN cd /etc/apt && \
  sed -i 's/archive.ubuntu.com/ftp.kaist.ac.kr/g' sources.list

RUN apt update -y

RUN apt install -y sudo vim wget tzdata
RUN apt install -y apache2

CMD [ "bash" ]
```

### Ref.
* <https://www.leafcats.com/242>
* <https://stynxh.github.io/2020-07-26-set-timezone-when-ubuntu-docker-image-build/>
