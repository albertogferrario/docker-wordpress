# Docker Wordpress w/ Swarm

## Create `.env`

```shell
cp example.env .env
```

## Create stack

```shell
export $(grep -v '^#' .env | xargs) && \
docker stack deploy -c .yml wordpress
```

