## Clone The Repository

### Newer versions of Git

```shell
git clone --recurse-submodules https://github.com/dttr278/heroes-deployment.git
```

### Older versions of Git

```shell
git clone --recursive https://github.com/dttr278/heroes-deployment.git
```

### Existing Checkouts

```shell
git submodule update --remote --checkout
```

## Config env

Create .env file in each submodule

## Run only one service

```shell
docker-compose create {service_name}
docker-compose start {service_name}
```

**Available service:**

- heroes-crontab-redeem
- heroes-ingame
- heroes-issue
- heroes-metadata

## Run all service in detach mode

```shell
docker-compose up -d
```

## Reference

- [Docker](https://docs.docker.com/engine/install/ubuntu/)
- [Docker compose](https://docs.docker.com/compose/install/)
