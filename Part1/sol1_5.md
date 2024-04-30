# Pulling images, compare sizes, and check secret message

```bash

mac@nanasmac ~ % docker images | grep "devopsdocker"
devopsdockeruh/simple-web-service   ubuntu         4e3362e907d5   3 years ago    83MB
devopsdockeruh/simple-web-service   alpine         fd312adc88e0   3 years ago    15.7MB
```

```bash
mac@nanasmac ~ % docker run -it -d --name task1-5 devopsdockeruh/simple-web-service:alpine
83fa92852e8c7cdcb73f3115133df64cbc0c01269b5f545247060279aa99e6c6
mac@nanasmac ~ % docker exec task1-5 tail -f ./text.log
2024-04-30 08:40:39 +0000 UTC
2024-04-30 08:40:41 +0000 UTC
Secret message is: 'You can find the source code here: https://github.com/docker-hy'
2024-04-30 08:40:43 +0000 UTC
2024-04-30 08:40:45 +0000 UTC
2024-04-30 08:40:47 +0000 UTC
2024-04-30 08:40:49 +0000 UTC
2024-04-30 08:40:51 +0000 UTC
Secret message is: 'You can find the source code here: https://github.com/docker-hy'
2024-04-30 08:40:53 +0000 UTC
2024-04-30 08:40:55 +0000 UTC
2024-04-30 08:40:57 +0000 UTC
```
