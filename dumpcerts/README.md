# Dumpcerts

See https://github.com/containous/traefik/blob/master/contrib/scripts/dumpcerts.sh

## Usage
```sh
docker run -it --rm \
  -v $(pwd)/acme.json:/in/acme.json \
  -v $(pwd)/out:/out/
  deluca/dumpcerts
```
