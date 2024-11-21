# Serve FastAPI app behind Nginx

## Quickstart

`docker compose up`

## Example `.env`

```shell
# url_pypi_index='https://artifact.xxx.com/repository/pypi-proxy/simple'
url_pypi_index='https://pypi.org/simple' ## official pypi repo from internet
# url_docker_index='artifact.xxx.com:999'
url_docker_index='docker.io' ## official docker repo from internetb-gitbucket/" # no space allowed

NGINX_PORT=80
```
