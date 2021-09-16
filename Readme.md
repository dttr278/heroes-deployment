## Clone The Repository
### Newer versions of Git
```shell
git clone --recurse-submodules https://github.com/dttr278/heroes-deployment.git checkout-path
```

### Older versions of Git
```shell
git clone --recursive https://github.com/dttr278/heroes-deployment.git checkout-path
```

### Existing Checkouts
```shell
git submodule update --remote --checkout
```

## Config env
Edit file in env folder with same name of sub module

## Run only one service
```shell
docker-compose create {service_name} 
docker-compose start {service_name}
```

__Available service:__
- heroes-crontab-redeem
- heroes-ingame
- heroes-issue
- heroes-metadata

## Run all service in detach mode
```shell
docker-compose up -d
``` 
