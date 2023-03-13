## Run Jenkins using docker compose with docker dind image

###### Tested on ubuntu-22.04 with arm64 arcitecture on aws

### Dockerfile in this folder will modify offical jenkins image to install docker-cli
```bash
docker build -t myjenkins-blueocean:2.387.1-1 .
```

### Use docker-compose.yaml in this directory
```bash
docker compose up -d
```

### Referance Page
https://www.jenkins.io/doc/book/installing/docker/
