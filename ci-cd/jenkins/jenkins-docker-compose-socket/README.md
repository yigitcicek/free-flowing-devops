## Run Jenkins on ubuntu-22.04 arm64 using docker compose

###### Tested on ubuntu-22.04 with arm64 arcitecture on aws

### Change docker socket permissions
```bash
sudo chmod 666 /var/run/docker.sock
```

### Dockerfile will modify offical jenkins image and install full docker stack
```bash
docker build -t my-jenkins:2.387.1-lts-1 .
```

### Compose up
```bash
docker compose up -d
```
