## Mongo and Mongo Express docker commands

```bash
docker network create mongo-network
```

```bash
docker run -d \
-p 27017:27017 \
-e MONGO_INITDB_ROOT_USERNAME=yadmin \
-e MONGO_INITDB_ROOT_PASSWORD=123qweASD \
--name = mongodb \
--net mongo-network \
mongo
```

```bash
docker run -d \
-p 8081:8081 \
-e ME_CONFIG_MONGODB_ADMINUSERNAME=yadmin \
-e ME_CONFIG_MONGODB_ADMINPASSWORD=123qweASD \
--net mongo-network \
--name mongo-express \
-e ME_CONFIG_MONGODB_SERVER=mongodb \
mongo-express
```
