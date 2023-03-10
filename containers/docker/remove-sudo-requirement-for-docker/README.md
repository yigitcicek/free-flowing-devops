## Remove sudo requirement for docker

###### Tested on ubuntu-22.04 arm64


##### Switch to desired user to run docker and apply the following commands
```bash
sudo usermod -aG docker ${USER}
su - ${USER}
sudo usermod -aG docker my_username
```

Refrence Page
https://www.digitalocean.com/community/tutorials/how-to-install-and-use-docker-on-ubuntu-22-04
