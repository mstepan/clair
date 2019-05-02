## Clair docker scanner

### Start clair server using docker compose.
```
./start-clair.sh
```

### Run clair scanner locally for `web-edge-server` docker image.
```
clair-scanner --ip 10.7.20.55 docker.va.opower.it/opower/web-edge-server:3.3.11-SNAPSHOT
```

### Run clair scanner locally for `multi-account-service` docker image.
```
docker pull docker.va.opower.it/services/multi-account-service:1.8.5
clair-scanner --ip 10.7.20.55 docker.va.opower.it/services/multi-account-service:1.8.5
```

### Additional resources to check.

1. https://github.com/arminc/clair-scanner
2. https://github.com/coreos/clair
