# Pulling image

```bash
docker pull devopsdockeruh/simple-web-service:ubuntu
docker run -it -d --name task1-3 devopsdockeruh/simple-web-service:ubuntu
```

# Secret message

```bash
docker exec task1-3 tail -f ./text.log
Secret message is: 'You can find the source code here: https://github.com/docker-hy'
2024-04-29 18:54:40 +0000 UTC
2024-04-29 18:54:42 +0000 UTC
2024-04-29 18:54:44 +0000 UTC
2024-04-29 18:54:46 +0000 UTC
2024-04-29 18:54:48 +0000 UTC
Secret message is: 'You can find the source code here: https://github.com/docker-hy'
2024-04-29 18:54:50 +0000 UTC
2024-04-29 18:54:52 +0000 UTC
2024-04-29 18:54:54 +0000 UTC
2024-04-29 18:54:56 +0000 UTC
2024-04-29 18:54:58 +0000 UTC
Secret message is: 'You can find the source code here: https://github.com/docker-hy'
2024-04-29 18:55:00 +0000 UTC
2024-04-29 18:55:02 +0000 UTC
2024-04-29 18:55:04 +0000 UTC
2024-04-29 18:55:06 +0000 UTC
2024-04-29 18:55:08 +0000 UTC
Secret message is: 'You can find the source code here: https://github.com/docker-hy'

```

> Secret message is: 'You can find the source code here: https://github.com/docker-hy'
