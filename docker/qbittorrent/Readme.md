### Support Info

Shell access whilst the container is running:

```
docker exec -it qbittorrent /bin/bash
```
To monitor the logs of the container in realtime:

```
docker logs -f qbittorrent
```
Container version number:

```
docker inspect -f '{{ index .Config.Labels "build_version" }}' qbittorrent
```

Image version number:

```
docker inspect -f '{{ index .Config.Labels "build_version" }}' lscr.io/linuxserver/qbittorrent:latest
```

