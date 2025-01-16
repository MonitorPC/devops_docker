`docker pull devopsdockeruh/simple-web-service:alpine`

`docker run -d -it --name secret devopsdockeruh/simple-web-service:alpin`

`docker exec -it secret sh`

`tail -f ./text.log` *inside container*

```
Secret message is: 'You can find the source code here: https://github.com/docker-hy'
2025-01-16 13:00:58 +0000 UTC
2025-01-16 13:01:00 +0000 UTC
2025-01-16 13:01:02 +0000 UTC
2025-01-16 13:01:04 +0000 UTC
2025-01-16 13:01:06 +0000 UTC
Secret message is: 'You can find the source code here: https://github.com/docker-hy'
2025-01-16 13:01:08 +0000 UTC
2025-01-16 13:01:10 +0000 UTC
2025-01-16 13:01:12 +0000 UTC
2025-01-16 13:01:14 +0000 UTC
2025-01-16 13:01:16 +0000 UTC
```
