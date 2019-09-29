# Docker Compose and WordPress

Build when Dockerfile has changed

```shell
docker-compose up -d --force-recreate --build
```

Cleanup

```shell
docker-compose rm -v
```

Recreate

```shell
docker-compose up -d --force-recreate
```

Rebuild docker container when Dockerfile has changed

```shell
docker-compose up -d --force-recreate --build
```
