# Dumpcerts

[![Docker Pulls](https://img.shields.io/docker/pulls/deluca/dumpcerts.svg)](https://hub.docker.com/r/deluca/dumpcerts/)

This container will monitor acme.json file for changes and run dumpcerts.sh if it happens. The container is using dumpcerts.sh from https://github.com/containous/traefik/blob/master/contrib/scripts/dumpcerts.sh

## Usage
```sh
docker run -it --rm \
  -v $(pwd)/acme.json:/in/acme.json \
  -v $(pwd)/out:/out
  deluca/dumpcerts
```
