# Docker

## Recipes

- Remove all stopped containers:

```bash
docker container prune

# or more old-fashioned way:
docker stop $(docker ps -a -q)
docker rm $(docker ps -a -q)

# another way with xargs
docker ps -a | grep Exit | cut -d ' ' -f 1 | xargs docker rm
```

- Remove unused images:

```bash
docker image prune

# or more old-fashioned way:
docker rmi $(docker images | grep "^<none>" | awk "{print $3}")
docker rmi -f $(docker images -qa -f 'dangling=true')
```

- Remove images, containers, networks and volumes:

```bash
docker system prune
```

- Filter container for specific image:

```bash
docker ps -a -q --filter ancestor="${IMAGE_NAME}" --format "{{.ID}}"
```
