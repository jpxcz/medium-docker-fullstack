# Fullstack docker development

## Depenencies

- docker
- docker-compose

## How tu run

```sh
$ docker-compose up --build
```

## Entry point

```sh
$ docker inspect -f '{{.Name}} - {{range .NetworkSettings.Networks}}{{.IPAddress}}{{end}}' $(docker ps -aq)
```
