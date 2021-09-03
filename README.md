# Laravel Docker with Nginx

## Requirement

- Docker version at least 18.06
- Docker compose version at least 1.22.0

## Setup development environment

### Environment variables

nginx in docker-compose.yml I use ports 80.

```shell
ports:
 - 80:80
```

If mysql you already use 3306 you can chnage to another port

```shell
mysql:
  ports:
    - 4306:3306
```

### Laravel (./src)


Make a **.env** file in src

```shell
cp .env.example .env
```

- `DB_HOST: mysql` 
- Configure your data base
  
