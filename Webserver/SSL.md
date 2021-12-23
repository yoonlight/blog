# SSL

## How to Apply?

* Use Docker

```shell
sudo docker run -it   --rm --name certbot \
  --mount src="{path}/conf",target=/etc/letsencrypt,type=bind \
  --mount src="{path}/lib",target=/var/lib/letsencrypt,type=bind \
  certbot/certbot certonly --manual \
  --preferred-challenges dns -d {example.com} -d *.{example.com}
```
